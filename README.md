# parse-online-csv-cell-lite

Used to quickly get the one cell value of online csv

> 可以用在線上的 csv檔 , 像是 google sheet 發布csv到網路上也可以使用

## How to use

 * import ``` https://kirinchen.github.io/parse-online-csv-cell-lite/poccl.js ```
 * useed it
 
 ```javascript
      fetchCSVCB('https://kirinchen.github.io/parse-online-csv-cell-lite/demo_color_srgb.csv',0,1,cell=>{
        // cell is value
		});
 ```
 
 ## Parameters
 
 1. url : csv file url
 2. pox : csv columns position
 3. poy : csv rows position
 4. cb : fetch data callback 
 
 ## example
 
 https://jsfiddle.net/tcfahdqL/13/
 
 code like :
 

 ```HTML
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
