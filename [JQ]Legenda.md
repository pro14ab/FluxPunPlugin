# [JQ]Legenda
##### Skrypt dodaje nam legendę grup pod listą osób które dziś odwiedziły forum.
![jpg](http://i.imgur.com/tLlkms7.png)

## Instalacja:
### PunBB
##### jQuery:
```sh
<script>
//Legenda by pro14ab
jQuery(document).ready(function(){
jQuery('#onlinetodaylist').after('<b>Legenda:</b><span id="Legenda_pro14"></span>');
jQuery('#Legenda_pro14').load('/userlist.php select[name="show_group"] option');
});
</script>
```
### FluxBB
##### jQuery:
```sh
<script>
//Legenda by pro14ab
jQuery(document).ready(function(){
jQuery('#onlinelist:nth-child(4)').after('<b>Legenda:</b><span id="Legenda_pro14"></span>');
jQuery('#Legenda_pro14').load('/userlist.php select[name="show_group"] option');
});
</script>
```
##### CSS:
```sh
#Legenda_pro14  option {display:inline-block;}
#Legenda_pro14  option[value="-1"]{display:none;}

/**
Zmiana koloru rang:
#Legenda_pro14  option[value="Z"]{color:X;}

Z-ID rangi (Admin-1   Mod-2  Użytkownik-4 i kolejne 5,6,7 itd.. )
X- kolor
**/
```