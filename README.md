# JavaScipt-Docs

# JavaScript Keywords
| abstract | final | protected |
|---|---|---|
| as | finally | public |
| boolean | float | return |
|break|for|short|
|byte|function|static|
|case|goto|super)|
|catch|if|switch|
|char|implements|synchronized|
|class|import|this|
|continue|in|throw|
|const|instanceof|throws|
|debugger|int|transient|
|default|interface|true|
|delete|is|try|
|do|long|typeof|
|double|namespace|use|
|else|native|var|
|enum|new|void|
|export|null|volatile|
|extends|package|while|
|false|private|with|

# Alert
```
alert("Hello World!");
```
# Variables
```
var name = "Idrees";
var nationality = "Pakistan";
var weight = "150";
var caseQty = 144;
```
# Math expressions
```
var commonNumber = 2 + 2;
var commonNumber = 12 - 24;
var commonNumber = 4 * 12;
var num = 10;
var commonNumber = 300;
var commonNumber = 15 / 4;
var remainder = 15 % 4;
```
### increment / decrement
```
num++; //post increment
num--; //post decrement
++num; //pre-increment
--num; //pre-decrement
num = num + 1;
num = num - 1;
```
### Eliminating ambiguity
```
var totalCost = 4*12+3+120*5;
var totalCost = 4*(12+3)*2+3 //123
var totalCost = 4*(12+3)*(2+3) //300
```
# Concatenating Text String
```
var message = "Assalamo Alaikum";
var name = "Idrees";
var username = "Norman"
alert(message +" "+ name)	//"Assalamo Alaikum Idrees"
alert("Thanks " + username)	//"Thanks Norman"
```
# Prompts
```
var name = prompt ("What's your name?");
var numberOfPets = prompt ("How many pets?");
```
# *if* statements
```
var x = prompt("What is the biggest continent in the world?");
if (x === "Asia") {
	alert("Correct");
}
```

### Comparision operators
\> is greater than
\< is less than
\>= is greater than or equal to
\<= is less than or equal to
\=== is equal to (match type and value both)
\== is equal to (math only value)
!== is not equal to (true if either the value or type does not match)
!= is not equal to (true if the value does not match regardless of the type)


```
if (1 > 0) {...code...}
if (0 < 1) {...code...}
if (1 >= 0) {...code...}
if (1 >= 1) {...code...}
if (1 <= 1) {...code...}
```
# *if*... *else* and *elseif* statements
### if (true)
```
var x = prompt("Which is the biggest continent in the world?");
if ( x === "Asia") {
	alert("Correct!");
}
```
### if (true) or if(false)
```
var x = prompt("Which is the biggest continent in the world?");
if ( x === "Asia") {
	alert("Correct!");
}
if (x !== "Asia") {
	alert("Wrong answer");
}
```
### if (true) or else
```
var x = prompt("Which is the biggest continent in the world?");
if ( x === "Asia") {
	alert("Correct!");
}
else {
	alert("Wrong answer");
}
```
### if, elseif, else
```
var correctAnswer = "Asia";
if (x === correctAnswer) {
	alert("Correct!");
}
elseif (x ==="Africa") {
	alert("Incorrect but close");
}
else {
alert ("Incorrect");
}
```
# Testing sets of conditions
Consider an School has a 100 meter running test for the criteria to qualify  to join sport team.

### SET I
```if (weight > 120 && time < 20) {...```
The above conditional statement checks two conditions that are combined with "**&&**" operator which literally means "**and**".  So, we can read the above conditional statement as " if a man has weight more than 120 pound **and** runs 100 meter under 20 sec, he can join school's sport team. Therefore, the both the conditions must be **true** to execute this block of code.
|weight > 120| time < 20|
|---|---|

### SET II
```if (weight > 120 && time < 20 && age > 17 && gender === "male") {...```
This set of conditions has four criteria, which are combined with "**&&**" that means all the four conditions must be **true** to meet the criteria.
|weight > 120| time < 20|age > 17|male|
|---|---|---|---|

### SET III
```if (SAT || avg || GPA > 2.5 || sport === "football") {...```

|SAT score avg |GPA > 2.5| sport football|
|---|---|---|

### SET IV
```if (age > 65 || age < 21 && res === "Pakistan") {...```

|age > 65 or age < 21 | Resident of Pakistan|
|---|---|

|age > 65 | age < 21 or Resident of Pakistan |
|---|---|

### SET V
```if ( (age > 65 || age < 21 ) && res === "Pakistan") {...```

|age > 65 or age < 21 | Resident of Pakistan|
|---|---|

### SET VI
```if (age > 65 || (age < 21 && res === "Pakistan") ) {...```

|age > 65 | age < 21 or Resident of Pakistan |
|---|---|

# *if* statements nested

Check out this code.
```
if ((x === y || a === b ) && c === d) {
	g = h;
}
else {
	e = f
}
```

and this (nested if statements)
```
if (c === d) {
	if(x === y ) {
		g = h;
	}
	else if (a === b) {
		g = h;
	}
	else {
		e = f;
	}
}
else {
	e = f;
}
```
<hr>

# Arrays
Assigning of some string values to some variabls.

```
var city0 = "Karachi";
var city1 = "Lahore";
var city2 = "Islamabad";
var city3 = "Faisalabad";
var city4 = "Multan";
var city5 = "Peshawar";
var city6 = "Quetta";
```
This is how we can create an array under a single container;

```
var cities = ["Karachi", "Lahore", "Islamabad", "Faisalabad", "Multan", "Peshawar", "Quetta"];
```

Mixed array
```
var mixedArray = [23, "Idrees", true, "2023"];
```

# Arrays: Adding and removing elements

You can assign or change a variable values whenever you like
```
var pets = [];
pets[0] = "dog";
pets[1] = "cat";
pets[2] = "bird";
pets[3] = "lizard";
pets[4] = "snake";

console.log(pets) // ['dog', 'cat', 'bird', 'lizard', 'snake']
```

## array.pop
Using the **pop** keyword, you can remove the last element of an array.

```
pets.pop();
console.log(pets)	//['dog', 'cat', 'bird', 'lizard']
```

## array.push
Using the **push** keyword, you can add one or more elements to the end of an array.

```
pets.push("fish", "ferret");
console.log(pets);	['dog', 'cat', 'bird', 'lizard', 'fish', 'ferret']
```

## array.shift
Use the **shift** method to remove an element from the beginning of an array.

```
pets = ['dog', 'cat', 'bird', 'lizard', 'fish', 'ferret'];
pets.shift();

console.log(pets);	//['cat', 'bird', 'lizard', 'fish', 'ferret'];
```

## array.unshift
use the **unshift** method to add one or more elements to the beginning of an array.

```
pets = ['cat', 'bird', 'lizard', 'fish', 'ferret'];
pets.unshift('lion', 'elephant');

console.log(pets)	//['lion', 'elephant', 'cat', 'bird', 'lizard', 'fish', 'ferret'];

```

## array.splice 

**using splice method to insert and remove simultaneously**
Use the **splice** method to insert one or more elements anywhere in an array, while optionally, removing one or more elements that come after it.
The following code 

```
pets = ['lion', 'elephant', 'cat', 'bird', 'lizard', 'fish', 'ferret'];
pets.splice(2, 2, "pig", "duck", "emu");

console.log(pets)	//['lion', 'elephant', 'pig', 'duck', 'emu', 'lizard', 'fish', 'ferret'];
```

in the above code, the first argument of splice method **2** the give elements (here; "pig", "duck", and "emu") to add from the index of **2**.
the second argument **2** means, to remove **2 items** next to it (here; "cat", "bird").
and the following arguments are the elements to be add.

**using splice method to insert new elements only**
you could make additions without removing any elements

```
pets = ['lion', 'elephant', 'cat', 'bird', 'lizard', 'fish', 'ferret'];
pets.splice(2, 0, 'pig', 'duck', 'emu');

console.log(pets)	//['lion', 'elephant', 'pig', 'duck', 'emu', 'cat', 'bird', 'lizard', 'fish', 'ferret'];
```

## array.slice
**use the slice method to copy one or more any consecutive elements in any position and put them into a new array**

```
pets = ['lion', 'elephant', 'cat', 'bird', 'lizard', 'fish', 'ferret'];
var newPets = pets.slice(2,4); // ['cat', 'bird'];

```

# for loops

```
for (var i = 0; i<=4; i++ ) {
	if (cityToCheck ===cleanestCities[i]) {
		alert("It's one of the cleanest cities");
	}
}
```

# for loops nested

```
var firstNames = ["Idrees", "Ishaq", "Hamza", "Usman", "Irfan"];
var lastNames = ["Ali", "Ahmed", "Siddiq", "Hashim"];
var fullNames = [];
for (var i = 0; i < firstNames.length; i++) {
	for (var j = 0; j < lastNames.length; j++) {
		fullNames.push(firstNames[i] +" "+ lastNames[j])
	}
}
console.log(fullNames);
```

# Changing case

## toLowerCase()
```
var cities = ["karachi", "HyderAbad", "LahOre", "PesHaWar", "IsLamABAD"];
var citiesInLowerCase = [];
for (var i =0 ; i < cities.length; i++ ) {
	citiesInLowerCase.push(cities[i].toLowerCase());
}
console.log(citiesInLowerCase);
```

## toUpperCase()

```
var cities = ["karachi", "HyderAbad", "LahOre", "PesHaWar", "IsLamABAD"];
var citiesInUpperCase = [];
for (var i =0 ; i < cities.length; i++ ) {
	citiesInUpperCase.push(cities[i].toUpperCase());
}
console.log(citiesInUpperCase);
```

# Strings: Measuring length and extracting parts

