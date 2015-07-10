### Startpage
***
Startpage is a simple homepage for your web browser that features random backgrounds.  
By default, it uses DuckDuckGo as its search engine.

Check it out [here](https://cdn.rawgit.com/fidelt/startpage/master/index.html).

### Changing the Backgrounds
***
- Replace all the images found in the **asset/background** directory with your images.
- Open the **index.html** file with a text editor.
- Now change the content of the **var backgrounds** to correspond to the names of your images.
```html
...
<script type="text/javascript" src="asset/js/bootstrap.min.js"></script>
<script>
	/* LIST YOUR IMAGES HERE */
	var backgrounds = [
			'Chrysanthemum.jpg',
			'Desert.jpg',
			'Tulips.jpg',
			];
	
	function GetRandomImg(active_indx) {
		var random_indx = Math.floor(Math.random() * $('.background').length);
...
```
- Finally, save the changes that you have made.

### Changing the Search Engine
***
- Open the **index.html** file with a text editor.
- Navigate to this part of the file:
```html
...
<div class="col-sm-8 col-sm-offset-2 grp">
	<form action="https://duckduckgo.com/" method="get">
		<div class="input-group">
			<input type="text" class="form-control" name="q" placeholder="Search DuckDuckGo">
			<span class="input-group-btn">
...
```
- Change the 'action' and 'placeholder' attributes of the form and input tags to your preferred search engine.

| Search Engine | action                             | placeholder     |
| ------------- | ---------------------------------- | --------------- |
| Bing          | `https://www.bing.com/search?`     | `Search Bing`   |
| Google        | `https://www.google.com/search?`   | `Search Google` |
| Yahoo!        | `https://search.yahoo.com/search?` | `Search Yahoo!` |
- Save the changes that you have made.
