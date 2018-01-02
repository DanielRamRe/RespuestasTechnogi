# Javascript Evaluation

1. What is a potential pitfall with using typeof bar === "object" to determine if bar is an object? How can this pitfall be avoided?

2. What will the code below output to the console and why?
   
```javascript
var myObject = {
    foo: "bar",
    func: function() {
        var self = this;
        console.log("outer func:  this.foo = " + this.foo);
        console.log("outer func:  self.foo = " + self.foo);
        (function() {
            console.log("inner func:  this.foo = " + this.foo);
            console.log("inner func:  self.foo = " + self.foo);
        }());
    }
};
myObject.func();
```

3. What is the significance of wrapping the entire content of a JavaScript source file in a function block?

4. What will the code below output to the console and why?
```javascript
 (function(){
    return typeof arguments;
  })();
```

5. What will the code below output to the console and why?
```javascript
  var foo = {
    bar: function() { return this.baz; },
    baz: 1
  };
  (function(){
    return typeof arguments[0]();
  })(foo.bar);
```

6. What will the code below output to the console and why?
```javascript
  var x = 1;
  if (function f(){}) {
    x += typeof f;
  }
  x;
```

7. What will the code below output to the console and why?
```javascript
/^(ab)$/.test('(ab)')
/^aa|bb$/.test('aaxx')
```


8. What is `use strict` used for?


9. Rewrite the following code as Ecmascript Arrow Function
```
var double = function (i) {
  return i * 2;
};
```


10. Using the following code
    ```
    
    function Logger(level){
        this.level = level
    }
    
    Logger.prototype.log = function(msg){
        console.log(this.level + ' ' +msg)
    }
    ```
    
    print to the console the text: `INFO Message`

11. Explain the difference between classical inheritance and prototypal inheritance.
