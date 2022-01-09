# SNOW-HTML
- this is a review of HTML

## Intro
- HTML stands for Hypertext Markup Language.
- It is a markup language for creating web pages and applications. 
- HTML contains a particular syntax - namely elements and attributes - that web browsers parse in order to render the content of the webpage. 
- With HTML, the structure and content of a webpage is defined. 
- Styling and dynamic behavior are introduced with CSS and JavaScript, respectively.

## Elements
- HTML is composed of many different elements – these provide the structure of the document. 
- Elements are defined within HTML files using tags
for example, one very common tag is the <div> tag. 
- The tag is enclosed within angle brackets. 
- Most elements have a closing tag which define the end of the element, using the backslash notation – 
for example, a closing "div" tag would be </div>. 
- HTML elements may be nested within other elements
- Not all elements have closing tags, some are self-closing. 
For example, the <img /> tag, which defines an image.

In order for HTML to be valid, tags must be properly nested - an outer tag cannot be closed before an inner one. 
For example, the following markup would not be considered valid:

## Attributes
- HTML elements can also have attributes defined within the tag - these are key/value pairs that give metadata about the tag that are important for the browser to know. 
- For example, image elements must have a URL which the browser can call to retrieve the image file to display on the page 
-we use the src attribute to do this: 
<img src="/URL/to/get/cat.png" alt="cool cat!" />.
 -As you may have guessed, the alt attribute specifies an alternative text to show when the image cannot be displayed.

## Global Attributes
### Global attributes are those that can be applied to any element on the page. Some important global attributes are:
- class
- id
- hidden
- lang
- style
- tabindex
- title
### There are also many attributes that should be applied to only certain elements, including the src and alt attributes shown above. 

## Starting HTML Documents
- Every HTML document (ending with .html extension) should begin with a special tag known as the DOCTYPE declaration 
- This lets browsers know what kind of document it is using (HTML, in our case) as well as which version of the markup language is being used. 
- For HTML5, the newest version and the one which we'll be using, the DOCTYPE syntax is:
![image](https://user-images.githubusercontent.com/12488769/148692585-5a9cc4e3-ed34-45b0-b3a2-5571b1941f2c.png)
- The doctype declaration tag does not have a closing tag and it is not self-closing either.
- The tag which begins the root of our HTML document is the <html> tag. 
- Everything about our webpage will be nested within this tag.
- Within the html element we have two important tags – 
- The <head> and the <body> tags. 
- The head element will contain all the metadata associated with this page, including the title, character encoding, and references to external stylesheets.
 - The body element contains the actual content of our page that will be rendered on the screen by the browser.

## Example
- meta tag defines the character encoding that the file will be using. 
- Also, the <!-- ... --> syntax denotes a comment.
![image](https://user-images.githubusercontent.com/12488769/148692657-00519ef9-6358-4461-aa1c-f33a443e7f0f.png)
 
## inline and block level elements
-  Block-level elements are those that will render on new lines in blocks by default, 
 - instead of rendering within the line itself like inline elements do. 
- One example of a block element is <div>, and a common inline element is <span>

## Common HTML elements
-  <div> - defines a "division of the page" 
- <p> - defines a paragraph 
- <span> - an inline tag for grouping text or elements 
- <b> - bold text 
- <i> - italicized text 
- <h1>, <h2>, ... <h6> - these are headings, h1 is largest and h6 is smallest 
- <br> - line break 
- <table> - defines a table 
- <img src="URL"> 
- <ol> - an ordered list 
- <ul> - an unordered list 
- <a href=""> - makes a hyperlink

 ## HTML Forms
 - An HTML form is a section of a document that contains controls such as text fields, password fields, checkboxes, radio buttons, submit button, menus, etc. 
- Using these elements the page can collect information from a user which is typically submitted to a web server. 
= To create a form, you would use the <form> tag.

## Why use a form
- We use forms to collect some information/data form the user. 
- For example: If a user wants to purchase some items on the internet, he or she must fill out the form which will collect information such as the shipping address and payment details so that the item can be sent to the given address
 
## Input element in forms
- An HTML form collects information from elements. 
- You will specify an addition type attribute to indicate which field to display. 
- Various fields can be created such as a text field, checkbox, password field, or radio button
 
 ## Text field
- A text field is a one-line input field that allows the user to input a line of text. 
- Text Fields are created by specifying the type attribute value as "text".
= The below example will display a text field with the label Email Id:
![image](https://user-images.githubusercontent.com/12488769/148692863-8a6aa85b-7e14-4063-98ea-128f5e176f31.png)

 ## Password field
 Password fields are a type of text field in which the text entered is masked using asterisk or dots. 
This prevents others form viewing the screen to see what is typed in. 
Also, its created by specifying the type attribute value as "password".

![image](https://user-images.githubusercontent.com/12488769/148692885-e8dd249a-3865-44f1-b4cd-5d9dc3f1ae73.png)

Although a password field is masked, it is NOT encrypted. 
You will have to use other measures such as HTTPS to encrypt data once the HTML form is submitted.

 ## Radio Buttons
 - Radio Buttons are used to let the user select exactly one value from a list of predefined options. 
- It is created by specifying the type attribute value as "radio".

- A form may have multiple sets of radio buttons. In order to make sure the user only selects one option from a given set, each radio element must have matching name attributes. 
- In the example above, both buttons have a name attribute value as gender.

## Checkboxes
 Checkboxes are used to let the user select one or more values from a pre-defined set of options. 
The type attribute value for checkboxes input control is "checkbox".


![image](https://user-images.githubusercontent.com/12488769/148692991-8618aad9-d565-4973-b027-1a5d28aff1e9.png)



Just like radio buttons, a form may have multiple sets of checkboxes. In order to make sure the user selects options related to a given set, each checkbox element must have matching name attributes. 
In the example above, each checkbox has a name attribute value as subject.

 ## File select boxes
- File select boxes are used to allow the user to select a local file on their computer and send it as an attachment to the webserver. 
- It is similar to a text box with a button that allows the user to browse for a file. 
- Instead of browsing for the file, the path and the name of the file can also be written. 
- They are created by specifying a type attribute value as "file".
 
 ![image](https://user-images.githubusercontent.com/12488769/148693024-535f67d9-1164-415a-9d87-30f502f2a3ba.png)

 

