The following notes serve as a roadmap of all the steps to complete the project.
For full documentation, refer to the final source code:

index.php
login.php
logout.php
build.php
queryLists.php
storeList.php
regester.php
header.php
login_form.php
profolio.php
register_form.php
footer.php
config.php
functions.php
constant.php
acupoint.js
radio_body.js
login.js
scripts.js
showLists.js
storeList.js
features.css
main.css
style.css

Topics covered:

Ajax
JQuery
PHP
Html
MySql
Event listeners
.css()
.val()
.html()
.prepend()
.append()
.clone()
.remove()
If...else...
Session
jQueryUI (.draggable())
Bootstrap (carousel, navbar, row of colums)

Log in:
Check if user has input the correct username and password. Also check if the text field is empty or not. After log in, the id and username will be stored in $_SESSION value. 

Sign up:
For new user to register an account. After sing up, the id and username will be stored in $_SESSION value.

Log out:
After log in with the correct username and password, the top right corner will show the log out button and the username. The $_SESSION will be destroyed. 

User status:
The functions of Build and Show acupoint pictures will open to those who have apply an account.

Dropdown menu:
The contents of dropdown menu includes General, Head, Back, Arms and Legs.
Step 1: Add the menu and style them.
Step 2: Write a dropdown listener for the menu.
Step 3: Introduce JavaScript variables to store the dropdown contents.
Step 4: Assign the #dropdown  a div which is already in the HTML.
Step 5: CSS cursor property (cursor:pointer;) to make the color blocks look clickable.


Radio button select:
The radio button is related to the selection of the dropdown menu. The contents are saved in the radio_body.js file.
Step 1: Add the related radio button and style them.
Step 2: Write a radio button listener for the menu.
Step 3: Introduce JavaScript variables to store the radio button.
Step 4: Assign the #radio_select, a div which is already in the HTML.
Step 5: CSS cursor property (cursor:pointer;) to make the color blocks look clickable.

Symptom description:
This input text will be added to the symptom description message.
Step 1: create a input element.
Step 2: Attach a key_up event to the input element.
Step 3: Use the .val() method to retrieve content entered in form elements; store the results in a variable.
Step 4: Use .html to put the message in the existing #recipients div in the canvas.
Step 5: Concatenate strings with the + operator to add an exclamation point to the end of the person's name.

Recipient Error checking
Step 1: Add a maxlength attribute on the recipient text field to limit the characters to 14.
Step 2: Use the JS .length String property to determine how many characters a user has entered; store the results in a variable.
Step 3: Show a countdown message of how many characters the user has left.
Step 4: Use an If...Else statement to toggle the color of the message depending on whether the user have enough characters left (grey) or not (red).

Chose the markers
Step 1: Add the 7 marker, and give them a click listener and sticker style.
Step 2: Use the .clone() method to duplicate the stickers on click.
Step 3: Use the .prepend() method add the cloned sticker to the canvas.

Draggable stickers
Step 1: Add jQuery UI to your page, right after the jQuery include.

<script type="text/javascript" src="https://ajax.googleapis.com/ajax/libs/jqueryui/1.10.3/jquery-ui.min.js"></script>
Step 2: Use the .draggable() interaction on the stickers.
Step 3: Contain the draggable elements to the canvas
