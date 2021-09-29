# JS syntax

```js
// Ternary operator

var isadult = (age < 18) ? 'tooyoung': 'old enough';

var exports = {
  publicPath: process.env.NODE_ENV === 'production'
    ? '/production-sub-path/'
    : '/'
}

// IF
if (1 < 2) {
    alert("jo")
}

switch (key) {
    case value:
        
        break;

    default:
        break;
}
// Change image


// Create new elements and populate it
<div id ="demo">some content</div>

<script>

  //creating a new paragraph

  var p = document.createElement("p");

  var node = document.createTextNode("Some new text");

  //adding the text to the paragraph

  p.appendChild(node);



  var div = document.getElementById("demo");

  //adding the paragraph to the div

  div.appendChild(p);

</script>


function setImage(base64) {
    document.getElementById("qr").src = base64
}


// Remove classes from all elements
eel.expose(make_button_visible);
function make_button_visible() {

    var elems = document.getElementsByClassName('nonactive');

    while(elems.length > 0){
        elems[0].classList.remove('nonactive');
    }

}


// Detect wrapped elements in flex
var detectWrap = function(className) {
    var wrappedItems = [];
    var prevItem = {};
    var currItem = {};
    var items = document.getElementsByClassName(className);
  
    for (var i = 0; i < items.length; i++) {
      currItem = items[i].getBoundingClientRect();
      if (prevItem && prevItem.top < currItem.top) {
        wrappedItems.push(items[i]);
      }
      prevItem = currItem;
    }

    return wrappedItems;

}

window.onresize = function(event){
var wrappedItems = detectWrap('flex-row');
for (var k = 0; k < wrappedItems.length; k++) {
    wrappedItems[k].className = "flex-wrapped";
}
}
```
# Vue

### Start new project

npm init
vue create my-app
vue add vuetify