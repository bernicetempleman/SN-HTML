# SNOW-HTML
- this is a review of HTML

## Intro
- HTML stands for Hypertext Markup Language.
- It is a markup language for creating web pages and applications. 
- HTML contains a particular syntax 
-  namely elements and attributes
-  that web browsers parse in order to render the content of the webpage. 
- With HTML, the structure and content of a webpage is defined. 
- Styling and dynamic behavior are introduced with CSS and JavaScript, respectively.

## Elements
```
- HTML is composed of many different elements
- these provide the structure of the document. 
- Elements are defined within HTML files using tags
for example, one very common tag is the <div> tag. 
- The tag is enclosed within angle brackets. 
- Most elements have a closing tag which define the end of the element, using the backslash notation – 
for example, a closing "div" tag would be </div>. 
- HTML elements may be nested within other elements
- Not all elements have closing tags, some are self-closing. 
For example, the <img /> tag, which defines an image.

In order for HTML to be valid, tags must be properly nested 
- an outer tag cannot be closed before an inner one. 
For example, the following markup would not be considered valid:
```
## Attributes
- HTML elements can also have attributes defined within the tag 
-  these are key/value pairs that give metadata about the tag that are important for the browser to know. 
- For example, image elements must have a URL which the browser can call to retrieve the image file to display on the page 
-we use the src attribute to do this: 
```
<img src="/URL/to/get/cat.png" alt="cool cat!" />
```
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
```
- The tag which begins the root of our HTML document is the <html> tag. 
```
- Everything about our webpage will be nested within this tag.
- Within the html element we have two important tags
```
- The <head> and the <body> tags. 
 ```
- The head element will contain all the metadata associated with this page, including the title, character encoding, and references to external stylesheets.
 - The body element contains the actual content of our page that will be rendered on the screen by the browser.

## Example
- meta tag defines the character encoding that the file will be using. 
- Also, the <!-- ... --> syntax denotes a comment.
![image](https://user-images.githubusercontent.com/12488769/148692657-00519ef9-6358-4461-aa1c-f33a443e7f0f.png)
 
## inline and block level elements
-  Block-level elements are those that will render on new lines in blocks by default, 
 - instead of rendering within the line itself like inline elements do. 
 ```
- One example of a block element is <div>, and a common inline element is <span>
```
## Common HTML elements
 ```
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
```
 ## HTML Forms
 - An HTML form is a section of a document that contains controls such as text fields, password fields, checkboxes, radio buttons, submit button, menus, etc. 
- Using these elements the page can collect information from a user which is typically submitted to a web server. 
```
 To create a form, you would use the <form> tag.
```
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

 ### Text Area
- A text area is a multi-line text input control which allows users to provide a paragraph or multiple lines of text. 
- It is created by using the "textarea" element.
```
- This is one of the few input controls that DO NOT use the <input> element.
```
- You can control the size of a text area by adding attributes "rows" and "cols" to specify the number of rows and columns of text it supports. 
- Most often text area elements are resizable, but the default size is managed by those two attributes.
![image](https://user-images.githubusercontent.com/12488769/148693791-32d53ded-2be7-49fa-9a8d-eba7b3d51312.png)
 
 ## Select Boxes (Drop-downs)
 - Select boxes are used to allow users to select one or more options from a drop-down list. 
 ```
- Select boxes are created by using two elements: <select> and <option>. 
- The <select> element defines a drop-down while list items are defined within the select element using <option> elements.
```
![image](https://user-images.githubusercontent.com/12488769/148693828-77a040cf-9dfd-42e9-b846-a354ba367a0d.png)

## select multiple attribute

- The multiple attribute is a boolean attribute.
- When present, it specifies that multiple options can be selected at once.
- Selecting multiple options vary in different operating systems and browsers:
- For windows: Hold down the control (ctrl) button to select multiple options
- For Mac: Hold down the command button to select multiple options
- Because of the different ways of doing this, and because you have to inform the user that multiple selection is available
![image](https://user-images.githubusercontent.com/12488769/148694046-668b5a30-2994-4029-909d-49f141e787b3.png)
![image](https://user-images.githubusercontent.com/12488769/148694049-debc105d-74d1-4006-a31a-19eb03868c08.png)

## Reset and Subnit buttons
- The submit button allows the user to send the form data to the web server. You can define a submit button by specifying the type attribute as "submit".
- The reset button is used to reset the form data and will display any default values. You can define a reset button by specifying the type attribute as "reset".
![image](https://user-images.githubusercontent.com/12488769/148694093-0c2bddda-72ae-4a2b-80b9-00d994b47b23.png)

## Attributes used in HTML forms
```
There are several attributes that you can use on the <form> tag and on <input> elements
```
- action
- target
- name
- method
- value
- placeholder
- required
![image](https://user-images.githubusercontent.com/12488769/148694119-c329f372-ed7a-42ba-b4d5-eec80807cdfd.png)

## The Action Attribute
- The action attribute indicates where the form data will be processed. 
- Typically the value is a URL of a server. 
- Generally, the form data is sent to a webpage on the webserver after the user clicks on the submit button.
- In the above code, after clicking on the submit button, the form data would be sent to a page called test.php.

## The Target Attribute
- The Target attribute is used to specify whether the submitted result will open in the current window, a new tab or on a new frame. 
- The default value used is "self" which results in the form submission in the same window. 
- To make the result display in a new browser tab, the value should be set to "blank".
- In the above code, after clicking on the submit button, the result will open in a new browser tab. 
- Most often this attribute is not present and the default value of "self" is used.

## Name Attribute
- The name attribute should be provided for each input element. 
- It is not required, but the value provides a label for the data once the form is submitted. 
- If the name attribute is not specified in an input field then the data of that field will not be sent.
- In the above code, after clicking the submit button, the form data will be sent to a page called /test.php. 
- The data sent will include the username and password fields.

## The Method Attribute
- The method attribute is used to specify the HTTP method used to send data while submitting the form. 
- There are only two options available: GET and POST.
- GET - When using the GET method, after the submission of the form, the form values will be visible in the address bar of the browser.
- POST – When using the POST method, after the submission of the form, the form values will NOT be visible in the address bar of the browser.

## The value attribute
- The value attribute specifies an initial value for an input field. 
- It also serves as the attribute to use when providing a button label for submit and reset input elements.
- In the above example, there are no default values.

## The placeholder attribute
- The placeholder attribute specifies a hint that describes the expected value of the input field (a sample value or a short description of the expected format). 
- The short hint is displayed in the input field before the user enters a value. 
- The placeholder attribute works with the following input types: text, search, url, tel, email, and password.
- In the above example, the text field has a placeholder of "Username".

## The required attribute
- The required attribute indicates an input field that must be filled out before submitting the form. 
= In most modern browsers, it will prevent the user from submitting the form until an acceptable value is entered. 
- The required attribute works with the following input types: text, search, url, tel, email, password, date pickers, number, checkbox, radio, and file.
- In the above example, only the text field is required.
- The required attribute doesn't have a value portion. You only need to specify the word 'required'.

## The min and max attribute
- The min and max attributes specify the minimum and maximum values for an input field. 
- The min and max attributes work with the following input types: number, range, date, datetime-local, month, time and week.
- Tip: Use the max and min attributes together to create a range of legal values. (For example: Set a maximum date or a minimum date)

![image](https://user-images.githubusercontent.com/12488769/148694329-7d267cf5-05f1-4285-a2dc-43a11c1dadbd.png)

# HTML5
```
HTML5 introduced a new DOCTYPE declaration <!DOCTYPE html> and the character encoding (charset) declaration <meta charset="UTF-8">. 
The <DOCTYPE> declaration is used to inform the browser about the version of HTML used in the document. 
It is known as the Document Type Declaration (DTD). 
It just instructs the browser about the document type. 
A character encoding is an approach of converting bytes into characters. 
For validating the HTML document, a program must choose a character encoding.
HTML5 also introduced features to allow us to embed audio and video files on the web page and provides the support to run JavaScript in the background.
```

## HTML5 Semantic elements
```
Semantic Elements defines the meaning for the web page rather than just presentation.
The HTML elements like <div> and <span> are not related to the content on the web page. This kind of elements are called as non semantic elements.
The HTML elements like <form>, <table>, and <article> are used to define the content and on the webpage. This kind of elements are called as semantic elements.
```
## Section
```
The HTML5 <section> tag defines a thematic grouping of content. 
In a document, we have sections like chapters, headers, footers, introduction, content, contact information, etc.
```
![image](https://user-images.githubusercontent.com/12488769/148694397-7f69683b-7b5d-44e7-a70d-576bae2de608.png)

## Article
```
The <article> element represents a section of content that forms an independent part of a document or site such as Forum post, Blog post, Newspaper article, etc.,

```
![image](https://user-images.githubusercontent.com/12488769/148694418-a568bbee-cba1-469d-a298-2bd78733f01b.png)

## Header
```
The <header> element specifies a header for a document or section.
```
![image](https://user-images.githubusercontent.com/12488769/148694436-ba3db675-2d16-49f6-934e-e8a7292f0c8d.png)

## Footer
```
The <footer> element used to define the footer for a document or section. 
It contains information about the author of the document, copyright information, links to terms of use, contact information, etc.
![image](https://user-images.githubusercontent.com/12488769/148694448-8678e386-a875-4718-b8f6-64e76fbca178.png)

```
 ![image](https://user-images.githubusercontent.com/12488769/148694451-6f31453c-4506-40d1-9f86-67944e8c79b5.png)

## Navigation
```
The <nav> element is for major navigation blocks that specify a set of navigation links.
```
![image](https://user-images.githubusercontent.com/12488769/148694487-3090a013-5367-44b1-9933-85921c00682e.png)

## Aside
```
The <aside> element is used to identify content that is related to the primary content of the web page. 
The content inside the <aside> element does not constitute the primary content of the page. 
For example, we can have author information, related links, related content, and advertisements.
```
![image](https://user-images.githubusercontent.com/12488769/148694502-b2fc8069-ab8d-438b-8b3b-ee0dd05e2a1e.png)

## HTML figure and figcaption Elements![image](https://user-images.githubusercontent.com/12488769/148694513-6a9d3a9a-4c42-466e-b78d-5a13a96cecfd.png)

```
The <figure> element describes some flow content, optionally with a caption, that is self-contained and referenced as a single unit from the main flow of the document. 
The <img> and <figcaption> elements are grouped in a <figure> element. 
We use the <img> element to insert an image on the web page. 
To add the visual explanation of the image, we need a caption for that image. 
This can be achieved in the HTML5 by using <figcaption> element.

```
![image](https://user-images.githubusercontent.com/12488769/148694524-cb2dfd45-48e1-4898-9627-635d7d9a7428.png)

## HTML5 Audio tag
```
The HTML5 <audio> element used to embed audio in a web page.






The <audio> element defines sound content and it has a controls attribute that adds audio controls, like play, pause, and volume. Any text within the <audio> and </audio> displayed on the browser only if the audio was not supported by the browser.
The <source> element defines the media resources for the audio files and it has attributes such as src and type. The src is used to specify the file format of the audio content and type specifies the media types that <audio> element supports.
```
![image](https://user-images.githubusercontent.com/12488769/148694554-78d2c854-a2ac-43bd-a5d3-03d49442a689.png)
![image](https://user-images.githubusercontent.com/12488769/148694558-50802e5b-249d-4ec9-86e8-a9e42e878cdc.png)

## HTML5 Video Tag
```
The <video> element used to embed a video on a web page, such as a movie clip or other video streams.
```
![image](https://user-images.githubusercontent.com/12488769/148694581-0a56a53a-842b-49f3-9f21-92d2b6ab85a5.png)
![image](https://user-images.githubusercontent.com/12488769/148694584-e6f879b7-cb3c-49e0-8248-6098e17bd62a.png)

## HTML5 Validation
```
When we submit a form, the data in the form will be sent to the server, before that we need to make sure that all the required details are filled out also in the correct format. 
The process of ensuring or validating the data before submitting to the server is called Client-side form validation.
"This field is required" (it can't be blank). 
"Please enter the valid phone number" (it should contain the only number). 
"Invalid email address" (it should be in "lmn@asd.com" format). 
"Your password must include one number, one uppercase letter, one lowercase letter, and one special character".

The browser displays the above messages by validating the data entered the registration form. 
It checks whether the data is in the correct format and satisfies the constraints set by the application or not. 
If the browser validates the data, then it is called as client-side validation. 
Validation done by the server is called as server-side validation.
There are two different types of client-side validation.
Built-in form validation - It uses HTML5 form validation features.
JavaScript validation - It is coded using JavaScript. This validation is completely customizable.

```
## Built-in form validation
- We have attributes that can be used with the form elements for validation. Some of the attributes are listed below:
- required: Used when the user must fill the field before submitting the form.
- minlength and maxlength: Used to specify the minimum and maximum length of the text.
- min and max: Used to specify the min and max values for the numerical fields.
- type: Defines the data should be a number or an email address or other predefined type.
- pattern: Defines a pattern (regular expression) the entered data needs to follow.
- If the data entered in a form satisfies the constraints are considered valid. 
- If not, it is considered invalid. 
- We use : valid and : invalid CSS pseudo-class to differentiate between valid and invalid input fields. 
- The:invalid CSS pseudo-class used to select and style form <input> elements whose value is invalid
```
-   according to the validation attributes specified in the <input> element. 
- Similarly, the :valid CSS pseudo-class selects and styles the vaild form input elements.
```



