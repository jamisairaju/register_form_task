# register_form_task
In this task i have created a register form. which consist of user_name, E-mail,password,and submit button.
This register form main structure is created by HTML. this consists of all input tags and body of web page.
To visualize this page we have used css. This styling is useful for providing beauty to the web page.
Finally js will perform some tasks.


HTML:-
<!DOCTYPE html>: This is the doctype declaration, which specifies the version of HTML being used.
<html lang="en">: This is the opening tag for the HTML document. The lang attribute specifies the language of the document, in this case, English.
<head>: This is the opening tag for the head section of the HTML document. The head section contains meta-information about the document, such as the character encoding, viewport settings, and links to external resources.
<meta charset="UTF-8">: This meta tag specifies the character encoding for the document, which is UTF-8 in this case.
<meta http-equiv="X-UA-Compatible" content="IE=edge">: This meta tag specifies the compatibility mode for Internet Explorer.
<meta name="viewport" content="width=device-width, initial-scale=1.0">: This meta tag sets the viewport properties for responsive design, ensuring that the webpage is displayed properly on different devices.
<link rel="stylesheet" href="style.css">: This link tag is used to link an external CSS stylesheet to the HTML document. The href attribute specifies the path to the CSS file.
<script src="app.js" defer></script>: This script tag is used to link an external JavaScript file to the HTML document. The src attribute specifies the path to the JavaScript file, and the defer attribute indicates that the script should be executed after the HTML document has been parsed.
<title>Register</title>: This is the title tag, which specifies the title of the HTML document that will be displayed in the browser's title bar or tab.
<body>: This is the opening tag for the body section of the HTML document. The body section contains the visible content of the webpage.
<div class="container">: This div element with the class "container" is used to group the form elements together.
<form action="" id="form">: This form element is used to create a form. The action attribute specifies the URL to which the form data will be submitted, and the id attribute provides a unique identifier for the form.
<h1>Register</h1>: This h1 element is used to display the heading "Register" on the webpage.
<div class="input-group">: This div element with the class "input-group" is used to group each input field and its associated label and error message together.
<label for="username">Username</label>: This label element is used to create a label for the username input field. The for attribute specifies which input field the label is associated with.
<input type="text" id="username" name="username">: This input element is used to create a text input field for the username. The type attribute specifies the type of input field, the id attribute provides a unique identifier for the input field, and the name attribute specifies the name of the input field.
<div class="error"></div>: This div element with the class "error" is used to display an error message for the username input field.
The same structure is repeated for the email, password, and confirm password input fields.
<button type="submit">Register</button>: This button element is used to create a submit button for the form.
</form>: This is the closing tag for the form element.
</div>: This is the closing tag for the div element with the class "container".
</body>: This is the closing tag for the body section of the HTML document.
</html>: This is the closing tag for the HTML document.



CSS:-
1. Background Styles:
The background color is defined as a linear gradient from a teal-like color to a shade of purple.
The background-attachment is set to “fixed,” which keeps the background stationary while scrolling.
2. Form Container (#form):

The form is centered both horizontally and vertically on the page.
It has a white background with rounded corners.
It has padding to create space between the content and the container edges.
3. Heading Styles (h1):

The heading (h1) is centered and has a color that corresponds to a shade of purple.
4. Button Styles (#form button):

The submit button has a purple background with white text.
It has rounded corners, padding, and a border.
The cursor changes to a pointer when hovering over the button.
The font size is relatively large.
The button occupies the full width of its container.
5. Input Group Styles (.input-group):

Input groups are displayed as columns and have a margin at the bottom for spacing.
Input fields have rounded corners, a larger font size, and padding.
The default input field border color matches the initial background color.
When focused, input fields lose the outline.
Error messages have a red color and a smaller font size, appearing below the input fields.
6. Success and Error Styles (.input-group.success and .input-group.error):

Input fields in a group with the “success” class have a green border color.
Input fields in a group with the “error” class have a red border color.
Overall, this stylesheet creates an elegant and visually appealing form with careful attention to spacing, color coordination, and responsive design. It seems to be designed for use with the “Poppins” font and features a color scheme dominated by shades of teal and purple.


JavaScript:-
1. The validateInputs() function starts by getting the value of each input field and trimming any whitespace. Then, it checks if each input is empty or invalid according to specific criteria.
2. If an input is invalid, the setError() function is called to display an error message and add the "error" class to the input field's parent element. If an input is valid, the setSuccess() function is called to remove any error message and add the "success" class to the input field's parent element. Finally, the function returns true if all inputs are valid, and false otherwise.

3. The setError() function takes an input element and an error message as arguments. It selects the input field's parent element and the error message element using the parentElement and querySelector() methods, respectively. Then, it sets the error message text and adds the "error" class to the input field's parent element while removing the "success" class.

4. The setSuccess() function takes an input element as an argument. It selects the input field's parent element and the error message element using the parentElement and querySelector() methods, respectively. Then, it removes any error message and adds the "success" class to the input field's parent element while removing the "error" class.

5. The validateEmail() function is a regular expression that checks if an email address is valid. Overall, this JavaScript code adds form validation to the registration form created in the HTML code. It ensures that each input field is filled out correctly before the form is submitted.
