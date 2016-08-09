# replace-anchor-links
This is the simple Jquery plugin that convert all text in url format within a paragraph into html anchor link format. This is very easy to use.

###Screenshot
![alt tag](https://github.com/waiyanhein/replace-anchor-links/blob/master/Screenshot%20(311).png)

###Dependencies
Only jquery is required to use this plugin

###How to use
Have a look at an example below.

####Step 1. Download replace_anchor_links.min.js file and add reference in html header section as below
```
<script type="text/javascript" src="/js/jquery.js"></script>
<script type="text/javascript" src="js/replace_anchor_links.min.js"></script>
```

####Step 2. Copy this html
```
<h3>First Paragraph</h3>
<p id="paragraph-1">This is a url or link, www.google.com in a paragraph.</p>
<h3>Second Paragraph</h3>
<p id="paragraph-2">This is a url or link, www.google.com-+** in a paragraph.</p>
<h3>Third Paragraph</h3>
<p id="paragraph-3">This is a url or link, http://google.com in a paragraph.</p>
<h3>Fourth Paragraph</h3>
<p id="paragraph-4">This is a url or link, https://www.google.com,+= in a paragraph. https://www.bing.com</p>
```
####NOTE: html attribute selector class or id must be unique

####Step 3. include this javascript code in script section
```
<script type="text/javascript">
$(function(){
	$('#paragraph-1').replaceAnchorLinks();
	$('#paragraph-2').replaceAnchorLinks();
	$('#paragraph-3').replaceAnchorLinks();
	$('#paragraph-4').replaceAnchorLinks();
})
</script>
```
####That's it. You are done. All the urls in the paragraph will be converted into html anchor links.
