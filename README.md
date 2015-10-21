# Mithrilizer
Sublime package for auto completions of common Mithril methods  
[Needs to be updated with Mithril 2.0 API]  
[Mithril](http://lhorie.github.io/mithril/index.html) is a client-side MVC lightweight Javascript framework created by Leo Horie

## Installation

### [Package Control](https://sublime.wbond.net/installation)

1. Open Package Control: `Preferences -> Package Control`
2. Select `Package Control: Install Package`
3. Type `Mithrilizer` into the search box and select the package to install it

## Usage

Once installed, you need to be on a page with the syntax set to Javascript

###m -> m()
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

###mi -> m('input')
will display:
```javascript
m('input[type=]', oninput:, value: )
```
More details on the use of m() [here](http://lhorie.github.io/mithril/mithril.html)

###ma -> m('a')
```javascript 
m('a[href=/myroute]', {config: m.route}, 'Myroute')
```
More details on the use of m() [here](http://lhorie.github.io/mithril/mithril.html)

###mm -> Mithril module  
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

###mp -> m.prop()
Will display:
```javascript
m.prop('initial value');
```
More details on the use of m.prop() [here](http://lhorie.github.io/mithril/mithril.prop.html)

###mw -> m.withAttr()
Will display:
```javascript
m.withAttr('string here', callback here)
```
More details on the use of m.withAttr() [here](http://lhorie.github.io/mithril/mithril.withAttr.html)

###mro -> m.route()
Will display:
```javascript
m.route({root Element, '/defaultRoute',
	'/route1': Module name

	});

m.route.mode = 'search/hash/pathname';
```
More details on the use of m.route() [here](http://lhorie.github.io/mithril/mithril.route.html)

###mreq -> m.request()
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

###md -> m.deferred()
Will display:
```javascript
m.deferred('initial value');
```
More details on the use of m.deferred() [here](http://lhorie.github.io/mithril/mithril.deferred.html)

###ms -> m.sync([])
Will display:
```javascript
m.sync([
	Array of promises
]);
```
More details on the use of m.sync() [here](http://lhorie.github.io/mithril/mithril.sync.html)

###mt -> m.trust()
Will display:
```javascript
m.trust(content);
```
More details on the use of m.trust() [here](http://lhorie.github.io/mithril/mithril.trust.html)

###mren -> m.render()
Will display:
```javascript
m.render(root Element, [
	'Children elements'
]);
```
More details on the use of m.render() [here](http://lhorie.github.io/mithril/mithril.render.html)

###mrd -> m.redraw()
Will display:
```javascript
m.redraw(true/false);
```
More details on the use of m.redraw() [here](http://lhorie.github.io/mithril/mithril.redraw.html)

###mrs -> m.redraw.strategy()
Will display:
```javascript
m.redraw.strategy('all/diff/none');
```
More details on the use of m.redraw.strategy() [here](http://lhorie.github.io/mithril/mithril.redraw.html#strategy)

###mst -> m.startComputation() and m.endComputation()
Will display:
```javascript
m.startComputation();

m.endComputation();
```
More details on the use of m.startComputation/m.endComputation [here](http://lhorie.github.io/mithril/mithril.computation.html)