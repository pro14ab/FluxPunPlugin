# [JQ]Avatar autora ostatniego postu
##### Skrypt dodaje nam avatar osoby która jako ostatnia napisała post w danym temacie

![jpg](http://i.imgur.com/bBCtVOz.png)

## Instalacja:
##### jQuery:
```sh
<script>
//Skrypt napisał pro14ab
jQuery(document).ready(function() {
jQuery('.blocktable:not(#vf) .tcr a').val(function(){
var pro14abavek = jQuery(this).attr('href');
jQuery(this).load(''+pro14abavek+' .postavatar:last');
});
});
</script>
```
##### CSS ver1.
```sh
.tcr img{border: 1px solid;
max-width: 40px !important;
max-height: 40px !important;
float:left;}

.tcr .postavatar{margin:0;}

.tcr .postavatar:empty{background: url("DOMYŚLNY AVEK") no-repeat;
background-size: 100% 100%;
width: 40px;
height: 40px;
border: 1px solid;
float:left;}
```

##### CSS ver2.
```sh
.tcr img{max-width: 40px !important;
max-height: 40px !important;
float:left;
box-shadow: 3px 3px 6px black;
border-radius:20px;
margin-right:8px;}

.tcr .postavatar{margin:0;}

.tcr .postavatar:empty{background: url("DOMYŚLNY AVEK") no-repeat;
background-size: 100% 100%;
width: 40px;
height: 40px;
max-width: 40px !important;
max-height: 40px !important;
float:left;
box-shadow: 3px 3px 6px black;
border-radius:20px;
margin-right:8px;}
```
