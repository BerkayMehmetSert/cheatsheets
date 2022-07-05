<h1 style="font-family: Roboto" align="center">
JSON CHEAT SHEET 
</h1>

<h3 style="font-family: Roboto">
Getting started 
</h3>

<h4 style="font-family: Roboto">
<code>Types</code> 
</h4>

<li style="font-family: Roboto">
<code>Number</code>:	Double precision floating-point 
</li>

<li style="font-family: Roboto">
<code>String</code>:	Series of characters
</li>

<li style="font-family: Roboto">
<code>Boolean</code>:	true or false
</li>

<li style="font-family: Roboto">
<code>Array</code>:	Ordered sequence of values 
</li>

<li style="font-family: Roboto">
<code>Value</code>:	String, Number, Boolean, null etc
</li>

<li style="font-family: Roboto">
<code>Object</code>:	Unordered collection of key/value pairs 
</li>

<li style="font-family: Roboto">
<code>null</code>:	Null or Empty 
</li>

<h4 style="font-family: Roboto">
<code>String</code> 
</h4>

<li style="font-family: Roboto">
<code>\"</code>:	Double quote 
</li>

<li style="font-family: Roboto">
<code>\\</code>:	Backslash
</li>

<li style="font-family: Roboto">
<code>\/</code>:	Forward slash
</li>

<li style="font-family: Roboto">
<code>\b</code>:	Backspace
</li>

<li style="font-family: Roboto">
<code>\f</code>:	Form feed
</li>

<li style="font-family: Roboto">
<code>\n</code>:	Newline 
</li>

<li style="font-family: Roboto">
	<code>\r</code>:	Carriage return 
</li>

<li style="font-family: Roboto">
	<code>\t</code>:	Tab 
</li>

<li style="font-family: Roboto">
	<code>\u</code>:	Trailed by four hex digits 
</li>

<h4 style="font-family: Roboto">
<code>Number</code> 
</h4>

<li style="font-family: Roboto">
<code>Integer</code>:	Digits 1-9, 0 and positive or negative
</li>

<li style="font-family: Roboto">
<code>Fraction</code>:	Fractions like 0.3, 3.9
</li>

<li style="font-family: Roboto">
<code>Exponent</code>:	Exponent like e, e+, e-, E, E+, E
</li>

<h4 style="font-family: Roboto">
<code>Objects</code> 
</h4>

```json
{
  "color": "Purple",
  "id": "210",
  "composition": {
    "R": 70,
    "G": 39,
    "B": 89
  },
  "empty_object": {}
}
```

<h4 style="font-family: Roboto">
<code>Array</code>
</h4>

```json
[
	"Red",
	"Green",
	"Blue"
]
```

<h4 style="font-family: Roboto">
<code>Array of objects</code> 
</h4>

```json
{
  "children": [
    {"name": "Jimmy Smith", "age": 15},
    {"name": "Sammy Sosa", "age": 12}
  ]
}
```

<h4 style="font-family: Roboto">
<code>2D Array</code>
</h4>

```json
{
  "my_sequences": [
    [1, 2, 3],
    [4, 5, 6],
    [7, 8, 9, 0],
    [10, 11]
  ]
}
```

<h4 style="font-family: Roboto">
<code>Object of objects</code>
</h4>

```json
{
	"my_objects": {
		"1": {"name": "Jimmy Smith", "age": 15},
		"2": {"name": "Sammy Sosa", "age": 12}
	}
}
```

<h4 style="font-family: Roboto">
<code>Nested</code>
</h4>

```json
{
  "Jack": {
    "id": 1,
    "name": "Franc",
    "salary": 25000,
    "hobby": ["a", "b"],
    "location": {
      "country": "A", "city": "A-A"
    }
  }
}
```

<h3 style="font-family: Roboto">
Access JSON in JavaScript 
</h3>

<h4 style="font-family: Roboto">
<code>Access Object</code> 
</h4>

```javascript
let myObject = {
  "name": "Jason",
  "last": "Doe",
  "age": 39,
  "gender": "M",
  "salary": 70000,
  "married": true
};

myObject.name:	"Jason"
myObject["name"]: "Jason"
myObject.age: 39
myObject.other:	undefined
myObject[0]: undefined
```

<h4 style="font-family: Roboto">
<code>Access Nested</code>
</h4>

```javascript
let myObject = {
  "ref": {
    "name": 0,
    "last": 1,
    "age": 2,
    "gender": 3,
    "salary": 4,
    "married": 5
  },
  "jdoe": [
    "Jason",
    "Doe",
    39,
    "M",
    70000,
    true
  ],
  "jsmith": [
    "Tom",
    "Smith",
    42,
    "F",
    80000,
    true
  ]
};

myObject.ref.age: 2
myObject["ref"]["age"]: 2
myObject.jdoe: ["Jason", "Doe", 39 ...]
myObject.jsmith[3]: "F"
myObject[1]: undefined
```

<h4 style="font-family: Roboto">
<code>Access Array of Objects</code>
</h4>

```javascript
let myArray = [
  {
    "name": "Jason",
    "last": "Doe",
    "age": 39,
    "gender": "M",
    "salary": 70000,
    "married": true
  },
  {
    "name": "Tom",
    "last": "Smith",
    "age": 42,
    "gender": "F",
    "salary": 80000,
    "married": true
  },
  {
    "name": "Amy",
    "last": "Burnquist",
    "age": 29,
    "gender": "F",
    "salary": 60000,
    "married": false
  }
];

myArray[0]: {"name": "Jason", ...}
myArray[1].name: "Tom"
myArray[1][2]: 42
myArray[3] :undefined
myArray[3].gender: TypeError: Cannot read...
```