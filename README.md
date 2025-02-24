# Version 1.0.0
Contains doT.js snippets.

# Installation
In order to install an extension you need to launch the Command Pallete (Ctrl + Shift + P or Cmd + Shift + P) and type Extensions. There you have either the option to show the already installed snippets or install new ones. Search for EmberJS es6 and install it.

# Supported languages (file extensions)
- JavaScript (.js)
- Javascript(ES6) Snippets for dotJS
- Below is a list of all available javascript snippets and the triggers of each one. The ⇥ means the TAB key. All the snippets are indented as per ESLint

# Why code snippets?
- A code snippet is like the boilerplate which can be used frequently. 
- The main advantage of code snippets is that they speed up the development work. 
- They are templates that make it easier to enter repeating code patterns

# Why template engine?
In your application, a template engine allows you to use static template files. An HTML file is supplied to a client by replacing variables in a template file with actual values at runtime. Designing an HTML page becomes easier with this method of working.

# doT.js 
doT.js was built in order to find the quickest and most compact JavaScript templating function possible, with a focus on performance in V8 and Node.js. 
It performs admirably in both Node.js and browsers.
## Features
1. There are no dependencies, and the 120 loc custom delimiters are exceptionally fast.
2. Evaluation at runtime.
3. Conditionals are supported. 
4. Runtime interpolation and compile-time evaluation. 
5. Partials and conditonal support.
6. Provides encoding. 
7. Array iterators.
8. Streaming-friendly whitespace - strip or presserve.
9. It's up to you whether you want to use it without logic or with reasoning.

# Installation
## For Node.js
- If you plan to use doT with Node.js, you can install doT with npm:
> npm install dot
- Then use require('dot') in your code.
## For browsers
- Include the javascript file in your source:
<script type="text/javascript" src="doT.js"></script>

# API
## doT.templateSettings - default compilation settings
You can customize doT by changing compilation settings. Here are the default settings:

doT.templateSettings = {
|Trigger |	Content|
|-------|----------|
  |`evaluate`:|    /\{\{([\s\S]+?)\}\}/g,|
  |`encode`: |     /\{\{!([\s\S]+?)\}\}/g,|
  |`use`:|         /\{\{#([\s\S]+?)\}\}/g,|
  |`define`:|      /\{\{##\s*([\w\.$]+)\s*(\:|=)([\s\S]+?)#\}\}/g,|
  |`conditional`:| /\{\{\?(\?)?\s*([\s\S]*?)\s*\}\}/g,|
  |`iterate`: |    /\{\{~\s*(?:\}\}|([\s\S]+?)\s*\:\s*([\w$]+)\s*(?:\:\s*([\w$]+))?\s*\}\})/g,|
  |`varname`:| 'it',|
  |`strip`:| true,|
  |`append`:| true,|
  |`selfcontained`:| false|

};

If you want to use your own delimiters, you can modify RegEx in doT.templateSettings to your liking.

## Here is the list of default delimiters:
|Trigger |	Content|
|-------|----------|
|`{{ }}`|	for evaluation|
|`{{= }}`|	for interpolation|
|`{{! }}`	|for interpolation with encoding|
|`{{# }}`	|for compile-time evaluation/includes and partials|
|`{{## #}}`	|for compile-time defines|
|`{{? }}`|	for conditionals|
|`{{~ }}`	|for array iteration|

# doT.template - template compilation function
Call this function to compile your template into a function.

function(tmpl, c, def)
- tmpl - template text
- c - custom compilation settings, if null, doT.templateSettings is used
- def - data for compile time evaluation

Data is the default parameter for the function, and its name is it. By altering doT.templateSettings.varname, you can change the names and amount of arguments.

# Functions
|Trigger |	Content|
|-------|----------|
|`-fn`|	function with no params functionName() {}|
|`-fn`|	function with 1 param functionName(param) {}|

# Snippets
|Trigger |	Content|
|-------|----------|
|`Compile template function`|
|`Compile template function - 1`|
|`Array - Template`|
|`Select List of Option`|
|`Unordered List`|
|`Ordered List`|
|`If`|
|`If Else`|
|`Function`|
|`Function Call`|
|`Loading External Scripts`|
|`Variables`|
|`Ternary Operator `|




-----------------------------------------------------------------------------------------------------------

## Working with Markdown

**Note:** You can author your README using Visual Studio Code.  Here are some useful editor keyboard shortcuts:

* Split the editor (`Cmd+\` on macOS or `Ctrl+\` on Windows and Linux)
* Toggle preview (`Shift+CMD+V` on macOS or `Shift+Ctrl+V` on Windows and Linux)
* Press `Ctrl+Space` (Windows, Linux) or `Cmd+Space` (macOS) to see a list of Markdown snippets

### For more information

* [Visual Studio Code's Markdown Support](http://code.visualstudio.com/docs/languages/markdown)
* [Markdown Syntax Reference](https://help.github.com/articles/markdown-basics/)

**Enjoy!**
