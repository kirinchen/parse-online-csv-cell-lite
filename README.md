# parse-online-csv-cell-lite

Used to quickly get the one cell value of online csv

## How to use

 * import ``` https://kirinchen.github.io/parse-online-csv-cell-lite/poccl.js ```
 * useed it
 
 ```javascript
      fetchCSVCB('https://kirinchen.github.io/parse-online-csv-cell-lite/demo_color_srgb.csv',0,1,cell=>{
        // cell is value
		});
 ```
 
 ## example
 
 https://jsfiddle.net/tcfahdqL/13/
 
 code like :
 
 HTML
 ```
 <!DOCTYPE html>
<HTML>
	<HEAD>
	</HEAD>
	<BODY>
		  This is jQuery App
      <div id='rid'></div>
<script src="https://code.jquery.com/jquery-3.6.0.slim.min.js" integrity="sha256-u7e5khyithlIdTpu22PHhENmPcRdFiHRjhAuHcs05RI=" crossorigin="anonymous"></script>
<script src="https://kirinchen.github.io/parse-online-csv-cell-lite/poccl.js"></script>
<script >

$(document).ready(function ()
{

     
     fetchCSVCB('https://kirinchen.github.io/parse-online-csv-cell-lite/demo_color_srgb.csv',0,1,cell=>{
			alert(cell);
      $('#rid').html(cell);
		});

     
});

</script>
	</BODY>
</HTML>
 ```
