# Introduction

I personaly think JavaScript is really cool but it's basic objects, like Strings or Arrays, lake of utility methods.

This script simply add methods to object prototypes for an easier and more comprehensible JavaScript source code.

# Examples:

## Strings

You have already asked yourself how to capitalize a String ?
In JavaScript we do this like: 

```this.charAt(0).toUpperCase() + this.slice(1)``` 

Way too long and not very comprehensible right ? 

JSExtends lets you do exactly the same with: ```my_string.capitalize()```

## Arrays

Same applies for arrays. Ever wonder who to remove an element from an array? Typical case is:

```
const index = this.indexOf(element);
if(index !== -1)
  this.splice(index, 1);
```

I absolutly don't want to write this piece of code everyting I want to remove something from an array.

Thanks to JSExtends you can simply do:
```
my_array.remove(my_element);
```
