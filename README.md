
#Linking Documents with the <script> Tag
After this lesson, you'll be able to:
+ Save JavaScript code to a .js file
+ Use script tags to add Javascript scripts to an HTML doc
+ Understand the connection between HTML, CSS, and JS as discrete parts of the front end of a web page that work together
+ Understand the concept of Separation of concerns

## Saving and Linking JavaScript
We’ve been using the console to play around and test JavaScript core concepts. What if we want to create JavaScript that we can save for later, or use to add dynamic interaction to our HTML/CSS website?

Well, first off, we can save our JavaScript as a text file with a .js extension. Go ahead and create a `my_script.js` file and open it up in Atom.

Let's create a basic program so that we can test that everything is working.

```
console.log("Hello, World");
```
Console logging is a way to print strings of text to the JavaScript console. If we aren't in the console itself, we'll use console.log() to print out strings.

Save the file in the same directory as the HTML and CSS files for your website. Now, how do we run it?

This is where all three different front-end coding languages - HTML, CSS and Javascript - come together. In order for us to link and run the JavaScript on our HTML web page, we need to tell the browser where our script is. This is done with the `<script>` element in our HTML page. Remember when you linked your CSS file to add style to your HTML page? Do the same for our `.js` file by adding the `<script>` element to the `<body>` of our HTML document:
```
...
The rest of the HTML
...
<script src="my_script.js"></script>
</body>
```

You can add as many different scripts as you like. The `src` property is versatile - you can give it the name of a file in the same folder as the HTML, or the path to a file in another folder, or even the url of a script that exists somewhere else.

After adding the script tag, save the HTML file and load it up in the browser. Check your console, and see your message printed out!

## Separation of Concerns
HTML, CSS, and JavaScript work together to create the dynamic web pages we see on the web today. We keep each in their own files, but linked together they provide structure, style and dynamic interactivity to the page.

In the early wild west days of the internet, it was common to see HTML, CSS, JavaScript together in one document. Browsers will still support this behavior - many examples and introductions you'll see online use inline styles and scripts. Having everything in one file made the code nearly indecipherable, a jumbled mess that was hard to understand and update when there were problems. HTML, CSS, and JavaScript play different roles, and keeping them in separate docs helps you and anyone who has to read your code understand what is happening.

Maintaining different files for HTML(structure), CSS(style) and JavaScript(logic) is referred to as separation of concerns. Keeping different roles separate helps developers on all kinds of projects, on the web or otherwise. Great developers don't just know how to solve problems with code - they keep their projects organized so they are easy to understand later. We'll use best practices from the start, so that you can build great habits.
