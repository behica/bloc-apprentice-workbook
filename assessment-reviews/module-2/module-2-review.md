# Module 2 Review Questions and Exercises

## Instructions

1. Click "edit" at the top of the page.
2. Fill in your answers below each question.
3. Save your changes and send a link to your mentor!

*Note: any topics from the first assessment should be reviewed in addition to the questions below!*

## CSS

### Questions

1. What is the box model? - This is how content and its surroundings interact with the view. Content -> Padding -> Border -> Margin
**2. What is the difference between block and inline elements? -  Block level always start on a new line, inline are on the same block.**
3. What is responsive design? - A view design concept wherein your web page layout responds depending on the size of the window size or device resolution it is being used on. ie. the ability to make your browser window narrower and watch a 3 column layout collapse into 1 seamlessly. 
4. Which selector is more specific, a tag selector or class selector? - Class.
**5. What does `box-sizing` do? - **
6. What's the difference between `relative` and `absolute` positioning? - Absolute is always in the same position. Ex. you set the position at 0px, 0px and it will always be anchored in the top left of the window/view regardless of how elements are positioned around it. Relative moves relative to the content around it.

### Exercises

1. Write a CSS rule to turn the background color of the link with the `.btn` class blue on hover:

  ```html
  <style>
  a:hover {
    background-color: blue;
  }
  </style>
  
  <a href="#" class="btn">Learn more</a>
  ```

**2. Write a CSS rule to give the `.container` a maximum width of `980px` when the browser window is wider than `1200px`:**

  ```html
  <style>
  .container {
  max-width: 980px;
  }
  </style>
  <div class="container">
    <h1>I'm a heading!</h1>
  </div>
  ```

3. Which text would be red in the following example?
Third paragraph

  ```html
  <style>
    section p:last-child {
      color: red;
    }
  </style>

  <section>
    <p>First paragraph</p>
    <p>Second paragraph</p>
    <p>Third paragraph</p>
  </section>
  <section>
    <p>First paragraph</p>
    <p>Second paragraph</p>
    <p>Third paragraph</p>
  </section>
  ```

4. Open this [JSBin](http://jsbin.com/qigiwuhepe/1/edit?html,css,output). Write a CSS rule using floats to make the HTML sample into a four column layout. Paste your udpated link below.
http://jsbin.com/ciperugayo/edit?html,css,output

## JavaScript

### Questions

**1. What is a callback?**
A function that is ran within / outside another function which uses it after it has been executed.

### Exercises

1. Write a function `filterLongWords()` that takes an array of words and an integer `num` and returns the array of words that are longer than `num`.
function filterLongWords(arrayOfWords, num) {
  newArray = [];
  for(var i = 0; i < arrayOfWords.length; i++){
    if(arrayOfWords[i].length > num){
    newArray.push(arrayOfWords[i]);
  }
  return newArray;
}

2. Write a function `charFreq()` that takes a string and builds a frequency listing of the characters contained in it. Represent the frequency listing as a Javascript object. Try it with something like `charFreq("abbabcbdbabdbdbabababcbcbab")`.


## DOM Scripting

### Questions

1. What does DOM stand for and what is it?
Document Object Model - it is the view of a web page or 'document' as converted into a series of 'nodes' which allows Javascript to navigate and interact with the document as a whole.

### Exercises

1. Write a JavaScript statement that finds the element with the ID, `next`, and saves it to a variable called `nextButton`:

  ```html
  <script>
  var nextButton = document.getElementById('next');
  </script>
  <a href="#" id="next" class="btn">Next</a>
  ```

2. Write another line that updates the text of `nextButton` to `"Next image"`.
<script>
nextButton.textContent = 'Next image';
</script>

3. Write another line that adds a click event listener to `nextButton` so that when it's clicked the browser alerts `"Next image coming up."`.
nextButton.addEventListener("click", alert('Next image coming up.');

## jQuery

### Questions

1. What is a JavaScript library and why do we use them?
2. What is jQuery for?

### Exercises

1. Write a statement to select all elements with the `.btn` class using a jQuery selector and save them to a variable called `buttons`:

  ```html
  <a href="#" id="next" class="btn">Next</a>
  <a href="#" id="beginning" class="btn">Beginning</a>
  <a href="#" id="previous" class="btn">Previous</a>
  ```

2. Write another line that adds a click event to the buttons that logs `'click'` to the console when the button is clicked. Use the jQuery syntax.

## Angular

### Questions

1. How is a framework different than a library?
2. What is a controller?
3. What is a view?
4. What is a single page application?
5. What is a directive in Angular?

## Git

### Exercises

1. Write a command to create a new branch called `bug-fix`.
2. If you're on the `master` branch, write a command to merge a branch called `bug-fix` into the `master` branch.
