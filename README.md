# RespuestasTechnogi

 ## 1.-
 
 The problem with this syntax is that null is also considered an object in javascript, it can be avoided by just checking if bar is null first and then if its an object. If it is NOT null and it is an object, then bar is indeed an object.
 
 ## 2.-
 
 The output woul look like this:
 
  outer func: this.foo = bar
  outer func: self.foo = bar
  inner func: this.foo = undefined
  ineer func: self.foo = bar
  
  This is because the variable self is defined in the outer function's scope and not in the inner function, so it returns undefined as it has no assigned value.
  
  ##3.-
  
  A JS source file wrapped in a function block can work as a library or as a "class". It also helps contain and manage variables in case they are ones with the same name in other files.
  
  ##4.-
  
  It simply returns "object" since typeof returns the type of the variable and arguments is an object available in every function
  
  ##5.-
  
  It will return "undefined" because no varibles have been passed to the function, making the zero index of arguments undefined.
  
  ##6.-
  
  The return value will be "1object". 1 being the value of the variable "x" and object being the type of variable declared within the function that concatenates the two together.
  
  ##7.-
  
  
 
 
