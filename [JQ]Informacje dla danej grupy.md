# [JQ]Informacje dla danej grupy
##### Kod daje nam możliwość wyświetlenia informacje tylko dla użytkowników, gości i administratorów + moderatorów.


## Instalacja:
##### Informacje dla gości:

```sh
<script>
jQuery(document).ready(function() {
jQuery("#navlogin").val(function() {
 jQuery('#nzalogowany').show();
});});
</script>
```
```sh
<div id="nzalogowany" style="display:none;">Tu wpisz informacje dla gości</div>
```

##### Informacja dla użytkowników:
```sh
<script>
jQuery(document).ready(function() {
jQuery("#navlogout").val(function() {
  jQuery('#zalogowany').show();
});});
</script>
```
```sh
<div id="zalogowany" style="display:none;">Tu wpisz informacje dla użytkowników</div>
```

##### Informacje dla administratorów i moderatorów:
```sh
<script>
jQuery(document).ready(function() {
jQuery("#navadmin").val(function() {
 jQuery('#admin').show();
});});
</script>
```
```sh
<div id="admin" style="display:none;">Tu wpisz informacje dla adminów i modów</div>
```