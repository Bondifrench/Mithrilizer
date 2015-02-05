# Mithrilizer
Sublime package for auto completions of common Mithril methods

[Mithril](http://lhorie.github.io/mithril/index.html) is a client-side MVC lightweight Javascript framework created by Leo Horie

Once installed, you need to be on a page with the syntax set to Javascript

###m for m()
will display:
```javascript
m('div',{
	style: { }, 
	config: 'function name'
	},[
		'Children'
	])
```
More details on the use of m() [here](http://lhorie.github.io/mithril/mithril.html)  

###mi for m('input')
will display:
```javascript
m('input[type=]', oninput:, value: )
```
More details on the use of m() [here](http://lhorie.github.io/mithril/mithril.html)

###ma for m('a')
```javascript 
m('a[href=/myroute]', {config: m.route}, 'Myroute')
```
More details on the use of m() [here](http://lhorie.github.io/mithril/mithril.html)

###mm for Mithril module  
Will display:
```javascript
var mymodule = {};

mymodule.vm = 'Object literal {} or function Constructor'

mymodule.controller = function (options) {
	mymodule.vm.init();
};

mymodule.view = function (ctrl) {
	return 'view here';
}
m.module(document.body, mymodule);
```
More details on the use of m.module() [here](http://lhorie.github.io/mithril/mithril.module.html)

###mp for m.prop()
Will display:
```javascript
m.prop('initial value');
```
More details on the use of m.prop() [here](http://lhorie.github.io/mithril/mithril.prop.html)

###mw for m.withAttr()
Will display:
```javascript
m.withAttr('string here', callback here)
```
More details on the use of m.withAttr() [here](http://lhorie.github.io/mithril/mithril.withAttr.html)

###mro for m.route()
Will display:
```javascript
m.route({root Element, '/defaultRoute',
	'/route1': Module name

	})
```
More details on the use of m.route() [here](http://lhorie.github.io/mithril/mithril.route.html)

###mreq for m.request()
Will display:
```javascript
m.request({
	method: 'GET/POST',
	url: '/user',
	dataType: ,
	callbackKey: ,
	type: ,
})
```
More details on the use of m.request() [here](http://lhorie.github.io/mithril/mithril.request.html)

###md for m.deferred()
Will display:
```javascript
m.deferred('initial value');
```
More details on the use of m.deferred() [here](http://lhorie.github.io/mithril/mithril.deferred.html)

###ms for m.sync([])
Will display:
```javascript
m.sync([
	Array of promises
]);
```
More details on the use of m.sync() [here](http://lhorie.github.io/mithril/mithril.sync.html)

###mt for m.trust()
Will display:
```javascript
m.trust(content);
```
More details on the use of m.trust() [here](http://lhorie.github.io/mithril/mithril.trust.html)

###mren for m.render()
Will display:
```javascript
m.render(root Element, [
	'Children elements'
]);
```
More details on the use of m.render() [here](http://lhorie.github.io/mithril/mithril.render.html)

###mrd for m.redraw()
Will display:
```javascript
m.redraw(true/false);
```
More details on the use of m.redraw() [here](http://lhorie.github.io/mithril/mithril.redraw.html)

###mrs for m.redraw.strategy()
Will display:
```javascript
m.redraw.strategy('all/diff/none');
```
More details on the use of m.redraw.strategy() [here](http://lhorie.github.io/mithril/mithril.redraw.html#strategy)

###mst for m.startComputation() and m.endComputation()
Will display:
```javascript
m.startComputation();

m.endComputation();
```
More details on the use of m.startComputation/m.endComputation [here](http://lhorie.github.io/mithril/mithril.computation.html)