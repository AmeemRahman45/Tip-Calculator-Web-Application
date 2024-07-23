<h1>💸 Tip Calculator 💸</h1>
<p>
    Welcome to the Tip Calculator! This handy web app helps you quickly and accurately calculate tips based on your bill amount and desired tip percentage.
</p>
<br>
<h3>🚀 Features</h3>
<ul>
    <li>🧮 Easy Calculation: Enter the bill amount and tip percentage to get the tip and total amount.</li>
    <li>🎨 Clean and Modern Design: User-friendly interface with a visually appealing background.</li>
    <li>🔄 Real-time Results: Instantly see the calculated tip and total amount after clicking the button.</li>
</ul>
<br>
<h3>🔧 Technologies Used</h3>
<ul>
    <li>HTML: Structure and layout.</li>
    <li>CSS: Styling and responsive design.</li>
    <li>JavaScript: Functionality for calculating and displaying the tip.</li>
</ul>
<br><br>
<h3>📋 Code Explanation</h3>
<ol>
    <li>
        <h4>HTML Structure</h4>
        <pre>
&lt;!DOCTYPE html&gt;: Defines the document type and version of HTML.
&lt;html lang="en"&gt;: Begins the HTML document and specifies English as the language.
&lt;head&gt;: Contains meta-information about the document, such as character encoding, viewport settings, and links to external resources.
    &lt;meta charset="UTF-8"&gt;: Sets the character encoding to UTF-8.
    &lt;meta name="viewport" content="width=device-width, initial-scale=1.0"&gt;: Ensures the page is responsive on all devices.
    &lt;title&gt;: Sets the title of the page that appears in the browser tab.
    &lt;link&gt;: Includes external resources such as fonts from Google Fonts and a stylesheet for styling.
&lt;/head&gt;
&lt;body&gt;: Contains the content of the webpage.
    &lt;div class="container"&gt;: A central container for aligning and styling content.
        &lt;h1 class="tipCalculator"&gt;: A heading for the tip calculator section, styled to stand out.
        &lt;form id="tipForm"&gt;: A form containing input fields for bill amount and tip percentage.
            &lt;label for="billAmount" class="billAmount"&gt;: A label for the bill amount input field.
            &lt;input type="number" id="billAmount" step="0.01" required&gt;: An input field for entering the bill amount.
            &lt;label for="tipPercentage" class="tipPercentage"&gt;: A label for the tip percentage input field.
            &lt;input type="number" id="tipPercentage" step="0.1" required&gt;: An input field for entering the tip percentage.
            &lt;button type="button" id="calculateBtn"&gt;: A button to trigger the calculation.
        &lt;/form&gt;
        &lt;div id="result"&gt;: A container for displaying the calculated tip and total amount.
            &lt;p id="tipAmount"&gt;: A paragraph element to display the tip amount.
            &lt;p id="totalAmount"&gt;: A paragraph element to display the total amount.
        &lt;/div&gt;
    &lt;/div&gt;
    &lt;script src="/js/script.js"&gt;&lt;/script&gt;: Links to an external JavaScript file that contains the logic for calculating and displaying the tip.
&lt;/body&gt;
        </pre>
    </li>
    <li>
        <h4>CSS Styling</h4>
        <pre>
body: Styles the background and centers the content vertically and horizontally.
    background-image: url('/img/dust-particles-wallpapers.jpg'): Sets a full-screen background image.
    background-size: cover: Ensures the image covers the entire background area.
    background-position: center center: Centers the background image.
.container: Styles the container that holds the content.
    text-align: center: Centers text inside the container.
    background-color: rgba(255, 255, 255, 0.9): Sets a translucent white background for better contrast.
    padding: 40px: Adds padding inside the container.
    border-radius: 10px: Rounds the corners of the container.
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1): Adds a subtle shadow for a 3D effect.
    width: 300px: Sets the width of the container.
    margin: auto: Centers the container horizontally.
form: Styles the form inside the container.
    display: flex: Aligns form elements vertically.
    flex-direction: column: Stacks form elements vertically.
    align-items: center: Centers form elements horizontally.
label: Styles the labels inside the form.
    display: block: Makes labels block-level elements.
    margin: 10px 0 5px: Adds margin around labels.
    text-align: center: Centers label text.
input: Styles the input fields inside the form.
    width: 100%: Makes input fields full-width.
    padding: 10px: Adds padding inside input fields.
    margin-bottom: 10px: Adds margin below input fields.
    border: 1px solid #ccc: Adds a border around input fields.
    border-radius: 5px: Rounds the corners of input fields.
    box-sizing: border-box: Ensures padding and border are included in the width and height.
    font-family: "Roboto", sans-serif: Uses a sans-serif font for input text.
    font-weight: 400: Uses normal font weight for input text.
    font-size: 16px: Sets the font size of input text.
button: Styles the button used to calculate the tip.
    background-color: #007bff: Sets a blue background color.
    color: white: Makes the button text white.
    border: none: Removes default button border.
    padding: 10px 20px: Adds padding inside the button.
    border-radius: 5px: Rounds the corners of the button.
    cursor: pointer: Changes the cursor to a pointer when hovering over the button.
    text-align: center: Centers button text.
    font-family: "Roboto", sans-serif: Uses a sans-serif font for button text.
    font-weight: 500: Uses medium font weight for button text.
    font-size: 16px: Sets the font size of button text.
    letter-spacing: 1.5px: Adds space between letters in button text.
    text-transform: uppercase: Makes button text uppercase.
button:hover: Styles the button when hovered over.
    background-color: #0056b3: Changes the button color on hover for a visual effect.
#result: Styles the container for the calculated tip and total amount.
    margin-top: 20px: Adds margin above the result container.
#result p: Styles the paragraphs inside the result container.
    font-family: "Roboto", sans-serif: Uses a sans-serif font for result text.
    font-weight: 400: Uses normal font weight for result text.
    font-size: 14px: Sets the font size of result text.
    letter-spacing: 0.5px: Adds space between letters in result text.
    margin: 5px 0: Adds margin around result paragraphs.
    padding: 3px: Adds padding inside result paragraphs.
.billAmount: Styles the bill amount label.
    font-family: "Roboto", sans-serif: Uses a sans-serif font.
    font-weight: 500: Uses medium font weight.
    font-size: 16px: Sets the font size of the label text.
    letter-spacing: 0.5px: Adds space between letters in the label text.
.tipPercentage: Styles the tip percentage label.
    font-family: "Roboto", sans-serif: Uses a sans-serif font.
    font-weight: 500: Uses medium font weight.
    font-size: 16px: Sets the font size of the label text.
    letter-spacing: 0.5px: Adds space between letters in the label text.
.tipCalculator: Styles the heading for the tip calculator section.
    font-family: "Montserrat", sans-serif: Uses a serif font.
    font-weight: 600: Uses semi-bold font weight.
    font-size: 30px: Sets the font size of the heading text.
    text-transform: uppercase: Makes heading text uppercase.
        </pre>
    </li>
    <li>
        <h4>JavaScript Functionality</h4>
        <pre>
document.getElementById('calculateBtn').addEventListener('click', function() {
    // Retrieve the value of the bill amount input field and convert it to a float
    const billAmount = parseFloat(document.getElementById('billAmount').value);

    // Retrieve the value of the tip percentage input field and convert it to a float
    const tipPercentage = parseFloat(document.getElementById('tipPercentage').value);

    // Check if either of the input values is not a number or if they are invalid
    if (isNaN(billAmount) || isNaN(tipPercentage) || billAmount <= 0 || tipPercentage < 0) {
        alert('Please enter valid numbers. Bill amount must be greater than zero and tip percentage cannot be negative.');
        return;
    }

    // Calculate the tip amount based on the bill amount and tip percentage
    const tipAmount = (billAmount * tipPercentage / 100).toFixed(2);
    
    // Calculate the total //

<hr>
