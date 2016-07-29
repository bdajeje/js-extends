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

I absolutly don't want to write this piece of code for every time I want to remove something from an array.

Thanks to JSExtends you can simply do:
```
my_array.remove(my_element);
```

## List a methods:

### Strings

* capitalize: change first letter of a string to be uppercased.
* empty: check if a string is empty (return true of false)
* toASCCI: remove all non-ASCII characters from the string

### Arrays

* pushIfValid: add element to an array only if element is valid (not null nor undefined)
* first: return fist element of array (or null if array is empty)
* last: return last element of array (or null if array is empty)
* size: alias for length. Length is more appropriate for the size of a string. For an array, asking for the size, not the length, if more comprehensible
* empty: check if an array is empty
* unique: return an array with no duplicates
* remove: remove an element from an array
