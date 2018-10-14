# [JQ]You
##### Skrypt wyswietla nazwe usera w miejscu diva

## Instalacja:
##### jQuery:
```sh
<script>
jQuery(document).ready(function() {
//"You" by pro14ab
 jQuery('ul.conl li:first strong').clone().appendTo('.you');
  jQuery('.you:empty').html('<b>gościu</b>')
});
</script>
```
##### HTML:
```sh
<span class="you"></span>
```