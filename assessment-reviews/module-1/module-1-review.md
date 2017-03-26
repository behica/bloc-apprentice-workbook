# Module 1 Review Questions and Exercises

## Instructions

1. Click "edit" at the top of the page.
2. Fill in your answers below each question.
3. Save your changes and send a link to your mentor!

## HTML

### Questions

1. What is HTML and what is it used for? - HTML is used to 'code' web pages in a markup read by browsers.
2. What is the difference between an ID and a class? - ID specific to a segment of code and can only be used once in a web page as an assignment. Class can be used to apply similar markups to a variety of elements.
3. What does it mean to write "semantic" HTML? - Using 'semantic' words to refer to a page's markup. Like `<nav>` for the navigation bar, or `<article>` for article content on a page. These can replace traditional `<div>` elements.

### Exercises

1. Write a paragraph tag with a class of "highlight" and content "Watch out!".
```
<p class="highlight">Watch out!</p>
```

2. Write an HTML image tag to show an image called `profile-picture.jpg`.
`<img src='profile-picture.jpg'>`

3. Write a link tag that links to http://google.com.
`<a href="http://google.com>Google</a>`

5. Write an complete standard HTML document outline (including a DOCTYPE, and `<html>`, `<head>`, and `<body>` tags).
```
<!DOCTYPE html>
<html>
<head>
<script src="main.js"></script>
<link rel="stylesheet" type="text/css" href="main.css">
</head>
<body></body>
</html>
```

6. Inside of the code for the previous exercise, write the appropriate tag to link to a script file called `main.js`.
7. Inside of the code for the previous exercise, write the appropriate tag to link to a stylesheet file called `main.css`.
8. Write a numbered list in HTML and list three of your favorite books.

```
<ol>
  <li>Jurassic Park</li>
  <li>Game of Thrones</li>
  <li>American Gods</li>
</ol>
```

9. Fix the indentation of the following HTML sample:

  ```html
  <div>
    <ul>
      <li>Item 1</li>
      <li>Item 2</li>
      <li>Item 3</li>
    </ul>
  </div>
  ```

## CSS

### Questions

1. What is CSS and what is it used for?
`CSS is Cascading Style Sheets, a markup language used to style HTML elements`

2. What is the CSS box model?
`The box model is how content, padding, borders and margin interact with one another in spacing and positioning.`

3. What's the difference between margin and padding?
`Margin is the space around boxes. Padding is the space within a box surrounding the content.`

### Exercises

1. Write a CSS rule to make the text of all `h1` tags red.
```
h1 {
  color: red;
  }
```

2. Write a CSS rule to make the background color of the link with `class="btn"` blue:

  ```
 <style>
  a {
    background-color: blue;
    }
 </style>
 
  html
  <a href="#" class="btn">Learn more</a>
  ```

3. Write a CSS rule to give the first paragraph in the following HTML a font size of `20px`, but not the second paragraph.

  ```
  <style>
  .jumbotron {
    font-size: 20px;
    }
  </style>
  
  html
  <header class="jumbotron">
    <p>Hello, World!</p>
  </header>

  <p>Welcome to this awesome website!</p>
  ```

## JavaScript

### Questions

1. What is a function? What are they used for?
`A function is a set of code defined within its own variable that can be grouped and recalled / executed when needed.`

2. What is the difference between `==` and `===`?
`== does not care about type, === ensures type and value. ex. a string of '2' is not equal to the integer 2, but using == allows them to be equal. === will not recognize the equality.`

3. What is the difference between global and local scope variables?
`global scope variables can be accessed from anywhere within the code set. local scope variables can only be accessed within the function that they are defined in, when that function is executed.`

4. What is a boolean value?
`boolean is either 'true' or 'false'`

5. What is an array?
`An array is a set of independent data contained within a variable. ex [1, 2, 3, 4, 5] is an array of numbers that can be evaulated as a whole or individually.`

### Exercises

1. Write a line that declares a variable called `myName` and set its value to your name.
`var myName = 'Behic';`

2. Write a loop that logs the numbers 1 through 10 to the console.
```
for(var i = 1; i <= 10; i++){console.log(i);}
```

3. Translate the following pseudocode into JavaScript: if `score` is greater than `3` and `lives` is greater than `0`, alert "You win!".
```
if(score > 3 && lives > 0){
alert("You win!");
}
```

4. Write a function `sayHello` that takes one argument, a name, and logs "Hello, <name>!" to the console. Then, call the function below the function definition and pass in your name as the argument.
```
function sayHello(name){
  return console.log("Hello " + name + "!");
}
sayHello('Behic');
```

5. What would the following script log to the console?
`This logs "Friday, Friday".`

  ```javascript
  var currentSong = "Call Me Maybe";

  function setSong(song) {
    currentSong = song;
  }

  setSong("Friday, Friday");

  console.log(currentSong);
  ```

6. What would the following script log to the console?
`This logs 10`

  ```javascript
  var add = function(a, b) {
    return a + b;
  }

  var result = add(3, 7);

  console.log(result);
  ```

7. What would the following script log to the console?
`This logs "Hello Sarah ! Goodbye Sarah !" -- so long as there are '+'s after 'name'`

  ```javascript
  var helloGoodbye = function(name) {
    return sayHello(name) + " " + sayGoodbye(name);
  }

  var sayHello = function(name) {
    return "Hello " + name " !";
  }

  var sayGoodbye = function(name) {
    return "Goodbye " + name " !";
  }

  console.log(helloGoodbye("Sarah"));
  ```

8. Write a function `findLongestWord()` that takes an array of words and returns the length of the longest one.
```
function findLongestWord(arrayOfWords) {
  var longestWord = 0;
  for(var i = 0; i < arrayOfWords.length; i++){
    if(arrayOfWords[i].length > longestWord){
      longestWord = arrayOfWords[i].length;
    }
  }
  return longestWord;
}
```

9. Define a function `sum()` that sums all the numbers in an array of numbers. For example, `sum([1,2,3,4])` should return 10.
```
function sum(arrayOfNum) {
var sum = 0;
  for(var i = 0; i < arrayOfNum.length; i++){
    sum += arrayOfNum[i];
  }
  return sum;
}
```
10. Write a function that takes a character (i.e. a string of length 1) and returns true if it is a vowel, false otherwise.
```
function vowel(char){
  if(char === 'a' || char === 'e' || char === 'i' || char === 'o' || char === 'u'){
    return true;
    } else {
    return false;
    }
}
```
11. Write the correct line to make `"Woof!"` show up in the console based on this script:
`pet.speak();`

  ```javascript
  var pet = {
    name: "Charles",
    goodDog: true,
    speak: function() {
      console.log("Woof!");
    }
  };
  ```

12. Using the same script as above, write the correct line to log the dogs name to the console.
`console.log(pet.name);`

## Command Line

### Questions

1. What is the command line and what is it used for?
`The command line is used to execute tasks / commands within a terminal environment. Change directories, create files, execute commands, etc.`

2. What does the command `ls` do?
`Lists the files and folders within your current directory.`

3. What does the command `pwd` do?
`This prints the current working directory to the console.`

4. What does the following command do: `cd my-cool-project`
`changes your current working directory to my-cool-project`

### Exercises

1. Write the command to make a new directory called "my-cool-project".
`mkdir my-cool-project`

2. Write the command to create a file called "index.html".
`touch index.html`

3. Write the command to delete a file called "main.css".
`rm main.css`

## Git

### Questions

1. What is Git and what is it used for?
`Git is a tool to help with version control of an application.`

2. What is the difference between a local repository and a remote repository?
`A local repo is on your currently used machine. A remote repo is located on a remote server like github.`

### Exercises

1. Write the command that you would use to create a new local Git repository.
`git init`

2. Write the command to stage a file called `index.html` to be committed.
`git add index.html`

3. Write the command to view the current status of the git repository.
`git status`
