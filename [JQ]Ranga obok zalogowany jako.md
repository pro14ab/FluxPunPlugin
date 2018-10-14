# [JQ]Ranga obok zalogowany jako
##### Skrypt dodaje range z forum bokok panelu "zalogowany jako"

## Instalacja:
##### jQuery:
```sh
<script>
jQuery(document).ready(function(){
var ranga = jQuery('#navprofile a').attr('href').split('=')[1];
jQuery('#brdwelcome .conl strong').append(' - <span id="pro14ranga"></span>');
jQuery('#pro14ranga').load('profile.php?action=view&id=' + ranga +' .inform:first p:first');
});
</script>
```
##### CSS:
```sh
#pro14ranga{display: inline-flex;}
#pro14ranga p{padding: 0;}
```