# JavaScript Snippets for Sublime 


### [cl] console.log

```javascript
console.log(${1:obj});
```


### [comment] 

```javascript
  //--------------------------------------------------------------
  // Start Partial Description
  //--------------------------------------------------------------
  // Source Code
  //--------------------------------------------------------------
  // End Partial Description
  //--------------------------------------------------------------
```


### [de] Debugger 

```javascript
debugger;
```

### [jquery-wds] Jquery Plugin Snippet

``` javascript
window.Foo_Object = {};
( function( window, \$, that ) {

    // Private variable
    var fooVariable = 'foo';

    // Constructor
    that.init = function() {
        that.cache();

        if ( that.meetsRequirements() ) {
            that.bindEvents();
        }
    };

    // Cache all the things
    that.cache = function() {
        that.\$c = {
            window: \$(window),
            fooSelector: \$( '.foo' ),
        };
    };

    // Combine all events
    that.bindEvents = function() {
        that.\$c.window.on( 'load', that.doFoo );
    };

    // Do we meet the requirements?
    that.meetsRequirements = function() {
        return that.\$c.fooSelector.length;
    };

    // Some function
    that.doFoo = function() {
        // do stuff
    };

    // Engage
    \$( that.init );

})( window, jQuery, window.Foo_Object );
```
### [map] Map function 

```javascript
	var data = ${1};
	data.map(function(item, index) {
		${2:// Code}
	});
```


### [prop] Prop function 

```javascript
	${1:functionName}: function (${2:arguments}) {
		${3}
	}
```



### [prop] query selector 

```javascript
	${1:document}.querySelector('${2:selector}');
```


### [prop] query selector all

```javascript
	${1:document}.querySelectorAll('${2:selector}');
```



## Contributing

1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -m 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request 
