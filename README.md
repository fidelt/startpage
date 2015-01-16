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
<script type="text/javascript" src="js/bootstrap.js"></script>
<script>
    // PUT YOUR IMAGES HERE
    var backgrounds = ['Chrysanthemum.jpg', 'Desert.jpg', 'Tulips.jpg'];
    
    function GetRandomImg(active_indx) {
        random_indx = Math.floor(Math.random() * $('.background').length);
...
```
- Finally, save the changes that you have made.
