# YouTwobe Video Viewer
A simple, single-page application that lets multiple people watch the same YouTube video simultaniously and comment and annotate on that video while playback remains sychronized.

### Technologies
This project is powered by Google's Firebase platform.
This project uses Mithril.js, Less.js, Mocha, Instabul, Webpack, and Firebase's JS client libraries. These packages are managed by NPM.

Developed by Team Firebase^(Not Sponsored)
Michigan Technological University
CS3141 - CS4711

---

### HTML Reference
HTML by itself has no dynamic features or logic. HTML is purley for defining a structure or skeleton. Syntactically, HTML is exactly the same as XML.

```HTML
<tag>
    <nestedTag attribute="value">Some Text That Renders To The Screen</nestedTag>
</tag> 
```

[W3Schools](https://www.w3schools.com/html/default.asp) has a decent HTML reference and curiculum. For the most part, just make sure that you close your HTML in the correct order and you should be fine.

### Mithril Note
Most of the HTML for this application is generated by Mithril and is actually written as virtual DOM definitions under `/js/views`. Mithril renders the page from this virtual DOM and generates most of the HTML dynamically.

---

### NPM Scripts
*`npm run-script dev-start`: Automatically build the project whenever files are changed. Ctrl + C in the terminal to exit.
*`npm run-script build`: Build the project for deployment to website
*`npm run-script test`: Run the testing suite
*`npm run-script test-coverage`: Run code-coverage analysis

### Building?
This project uses Webpack to build a production ready application. Essentially, webpack will take all the js source files which are `require();`d in the application and generate a single Javascript file `bin/app.js` that contains all the application code. During this process it optimizes code and transpiles ES6 code which is not yet supported by most (any?) browsers inot ES5 code which the modern browsers can understand.