# coolfeatures-js

Cool features missing in JavaScript

## Features

### `Coolfeatures.getRandomArrayValue()`

The `getRandomArrayValue()` method returns a random value from the given array.

#### Demo

```javascript
const array1 = [1, 2, 3, 4];

console.log(Coolfeatures.getRandomArrayValue(array1));
// expected output: 1, 2, 3, or 4
```

#### Syntax

`var randomElement = Coolfeatures.getRandomArrayValue(array)`

##### Parameters

**`array`**<br>
The array where a random element should be selected from.

##### Return value

A random selected element from `array`.

<br>

### `Coolfeatures.filterObject()`

The `Coolfeatures.filterObject()` method creates a new object with all elements that pass the test implemented by the provided function.

#### Demo

```javascript
const personAges = {
    hans: 45,
    peter: 33,
    jens: 68,
    mike: 21
};

console.log(Coolfeatures.filterObject(personAges, age => age < 40));
// expected output: {peter: 33, mike: 21}
```

#### Syntax

`var newObject = Coolfeatures.filterObject(object, callback([element[, key[, object]]]))`

##### Parameters

**`object`**<br>
The object to filter.

**`callback`**<br>
Function is a predicate, to test each element of the object. Return true to keep the element, false otherwise. It accepts three arguments:

&ensp;**`element`**<br>
&ensp;The current element being processed in the object.

&ensp;**`key`**<br>
&ensp;The key of the current element being processed in the object.

&ensp;**`object`**<br>
&ensp;The object `Coolfeatures.filterObject` was provided with.

##### Return value

A new object with the elements that pass the test. If no elements pass the test, an empty object will be returned.

<br>

### `Coolfeatures.isObjectEmpty()`

The `isObjectEmpty()` checks an object for being empty.

#### Demo

```javascript
const emptyObject = {};

console.log(Coolfeatures.isObjectEmpty(emptyObject));
// expected output: true

const filledObject = {empty: false};

console.log(Coolfeatures.isObjectEmpty(filledObject));
// expected output: false
```

#### Syntax

`var objectIsEmpty = Coolfeatures.isObjectEmpty(object)`

##### Parameters

**`object`**<br>
The object to check for being empty.

##### Return value

`true` if the object is empty, otherwise `false`.

<br>

### `Coolfeatures.getRandomIntBetween()`

The `getRandomIntBetween()` method returns a random number between two given numbers.

#### Demo

```javascript
console.log(Coolfeatures.getRandomIntBetween(5, 10));
// expected output: a number between 5 and 10
```

#### Syntax

`var randomInt = Coolfeatures.getRandomIntBetween(min, max)`

##### Parameters

**`min`**<br>
The lowest possible random-generated number.

**`max`**<br>
The highest possible random-generated number.

##### Return value

A random number between the given min and max number.

<br>

### `Coolfeatures.htmlStringToElement()`

The `htmlStringToElement()` method parses a HTML string to an `Element`.

#### Demo

```javascript
const html = '<div id="my-div">Hello World!</div>'

console.log(Coolfeatures.htmlStringToElement(html));
// expected output: a new HTMLDivElement whose outerHTML is like html
```

#### Syntax

`var element = Coolfeatures.htmlStringToElement(htmlString)`

##### Parameters

**`htmlString`**<br>
The HTML string to convert to an element.

##### Return value

A new `Element` that got parsed from `htmlString`.