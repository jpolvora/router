# router
javascript vanilla router

###installation###
```html
<script src="router.js"></script>
```
###usage###
```javascript
var router = Jone.Router;

router.on("#!", function() {
    console.log('your are on the root route!');
});

router.on('#!path/to/your/hash', function() {
    console.log('hello!');
});

router.notfound(function(hash){
  console.log('hash not defined: ' + hash);
});

router.start();
```
###conventions###
All route definitions must start with ```"#!"```
###Features###
Parameter binding into callback
All 
###API###
```.on(/*string*/ hash, /*function*/ callback)```: Inserts a route in the router
```router.start();``` Starts listening to route events
```javascript
router.stop();
```
Stops listening route events
```javascript
router.clear();
```
Clear all routes

