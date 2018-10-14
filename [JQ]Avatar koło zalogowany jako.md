# [JQ]Avatar koło "zalogowany jako"
##### Skrypt dodaje nasz avatar koło "zalogowany jako..."
![jpg](http://i.imgur.com/PCgSt4d.png)

## Instalacja:
##### jQuery:
```sh
<script>
///Skrypt avatra by pro14ab
jQuery(document).ready(function(){
var IDuser = jQuery('#navprofile a').attr('href').split('=')[1];
jQuery('#brdwelcome .conl').before('<div id="proavatar"></div>');
jQuery('#proavatar').load('/profile.php?section=personality&id=' + IDuser +' #profileavatar img');
});
</script>
```
### PunBB
##### CSS:
```sh
#proavatar{float:left;margin-top: 3px;margin-right: 4px;}
#proavatar img{height: 30px;width: 30px;max-width: 30px;max-height: 30px; border-radius:3px;}

/** 
Jeżeli user nie posiada avatara można ustawić domyślny:
#proavatar:empty{background-image: url("LINK DO OBRAZKA");height: 30px;width: 30px; background-size: cover;margin-top: 3px;margin-right: 4px;border-radius:3px;}
**/
```

### FluxBB
##### CSS:
```sh
#proavatar{float: left;margin-top: -3px;margin-right: 4px;}
#proavatar img{height: 30px;width: 30px;max-width: 30px;max-height: 30px; border-radius:3px;}

/** 
Jeżeli user nie posiada avatara można ustawić domyślny:
#proavatar:empty{background-image: url("LINK DO OBRAZKA");height: 30px;width: 30px; background-size: cover;margin-top: -3px;margin-right: 4px;border-radius:3px;}
**/
```