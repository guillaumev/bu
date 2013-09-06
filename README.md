Browser Update
==

This is a clone of the script located at http://browser-update.org. This clone will allow you to use the browser update
script from an https website.

How to Use
==
Use the following javascript code to add the browser-update notification:

<script type="text/javascript"> 
var $buoop = {} 
$buoop.ol = window.onload; 
window.onload=function(){ 
 try {if ($buoop.ol) $buoop.ol();}catch (e) {} 
 var e = document.createElement("script"); 
 e.setAttribute("type", "text/javascript");
 if (window.location.protocol == "https:") {
   e.setAttribute("src", "https://raw.github.com/guillaumev/bu/master/update.js");
 }
 else {
   e.setAttribute("src", "http://browser-update.org/update.js"); 
 }
 document.body.appendChild(e); 
} 
</script> 
