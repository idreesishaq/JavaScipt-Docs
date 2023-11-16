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

