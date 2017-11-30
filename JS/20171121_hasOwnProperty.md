# JS Notes
##### 21st Nov. 2017

keywords: hasOwnProperty for loop in

### for loop vs. for ... in
In the following code, I was trying to rewrite the for loop with for ... in:

```
for (var i = 1; i < primitives.length; i++) {
  var object = primitives[i];
  var targetEntity = object.id;
  var globeId = targetEntity._name;
  var b = false;

  for (var j = 0; j < listID.length; j++) {
    if (!(-1==globeId.split('-').indexOf(listID[j]))) {
    b = true;
    entityCollection.push(targetEntity);
    }
  }
}
```
replace that with

```
for (const prim in primitives) {
  const targetEntity = prim.id;
  const globeId = targetEntity._name;
}
```
However it doesn't work: ._name couldn't be found; As...
[read this](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/for...in)

It's a bad idea to use for .. in loop in an array, as 

+ It doesn't execute in sequence of index
+ It may get objects out of expectation which is difficult to debug.

 
If need to use for .. in loop, remember to check "hasOwnProperty":

```
for (const prim in primitives) {
  if (primitives.hasOwnProperty(prim)) {
    // Do something here
  }
}
```

