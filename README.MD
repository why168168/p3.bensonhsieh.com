Topics covered:

Ajax
Event listeners
.css()
.val()
.html()
.prepend()
.append()
.clone()
.remove()
If...else...
jQueryUI (.draggable())
The following notes serve as a roadmap of all the steps to complete the project.
For full documentation, refer to the well-commented final source code:

index.html (Use View Source to see HTML code)
radio_body.js
acupoint.js
features.css
main.css

Open the following files in your code editor:

/index.html
/css/features.css
/css/main.css
/js/acupoint.js
/js/radio_body.js

body.gif
circle.png
arrow.png
face.png

Color chooser
Step 1: Add the color blocks and style them.

Step 2: Write a click listener for the color blocks.

Figure out what color was clicked using $(this):

In many object-oriented programming languages, this (or self) is a keyword which can be used in instance methods to refer to the object on which the currently executing method has been invoked. -wikipedia

jQuery ¡§this¡¨ keyword

Step 3: Introduce JavaScript variables to store the color.

Step 4: Assign the color to #canvas, a div which is already in the HTML.

Step 5: CSS cursor property (cursor:pointer;) to make the color blocks look clickable.

Textures chooser
Step 1: Add the 4 texture blocks and style them.

Step 2: Write a click listener for the texture blocks.

Step 3: Make the color picker also change the color of the texture blocks.

Bonus: Add one more texture to your options.

Message
Step 1: Add the 4 message radios, each with the name='message' and a unique id.

Step 2: After each radio, create a label element.

Give each label a for attribute to match the id of the radio it's labeling.

Step 4: Attach a click event to the radio buttons.

Step 5: Note there's a div with the id #message already in the #canvas. Use .html() to put the message in that div.

(Bonus) Font chooser
Add an option that lets you choose the font of your message

Recipient
Step 1: Add a text input.

Step 2: Attach a keyup event to that text input.

Step 3: Use the .val() method to retrieve content entered in form elements; store the results in a variable.

Step 4: Use .html to put the message in the existing #recipients div in the canvas.

Step 5: Concatenate strings with the + operator to add an exclamation point to the end of the person's name.

Recipient Error checking
Step 1: Add a maxlength attribute on the recipient text field to limit the characters to 14.

Step 2: Use the JS .length String property to determine how many characters a user has entered; store the results in a variable.

Step 3: Show a countdown message of how many characters the user has left.

Step 4: Use an If...Else statement to toggle the color of the message depending on whether the user have enough characters left (grey) or not (red).

Bonus: If you go back and delete the recipient, you're left with just an exclamation point on the card. Make it so this only shows if the user has something typed in.

Hint: var validate = recipient.replace(" ", "", recipient);

Stickers
Step 1: Add the 6 stickers, and give them a click listener.

Step 2: Use the .clone() method to duplicate the stickers on click.

Step 3: Use the .prepend() method add the cloned sticker to the canvas.

Draggable stickers
Step 1: Add jQuery UI to your page, right after the jQuery include.

<script type="text/javascript" src="https://ajax.googleapis.com/ajax/libs/jqueryui/1.10.3/jquery-ui.min.js"></script>
Step 2: Use the .draggable() interaction on the stickers.

Step 3: Contain the draggable elements to the canvas