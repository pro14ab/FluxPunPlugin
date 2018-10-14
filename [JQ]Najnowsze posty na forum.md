# [JQ]Najnowsze posty na forum
##### Kod pokazuje 30 najnowszych postów w przeciągu 24 godzin.


## Instalacja:
##### jQuery:
```sh
<script>
//Najnowsze posty by pro14ab
jQuery(document).ready(function() {
  jQuery('#brdstats').after('<H2>Najnowsze posty:</H2><div style="overflow:scroll;overflow-x:hidden;height:200px;margin-bottom: 15px;"><div id="najnowsze_pro14ab"></div></div>');
  jQuery('#najnowsze_pro14ab').load('search.php?action=show_24h #vf');
});
</script>
```
##### CSS:
```sh
#najnowsze_pro14ab #vf h2{display: none; }
#najnowsze_pro14ab #vf thead{display: none; }
#najnowsze_pro14ab #vf td.tc2{display: none; }
#najnowsze_pro14ab #vf td.tc3{display: none; }
#najnowsze_pro14ab #vf span{display: none; }
#najnowsze_pro14ab #vf  DIV.inbox DIV {PADDING: 0px 0;}
```

