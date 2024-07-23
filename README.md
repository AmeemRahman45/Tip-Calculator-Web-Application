<h1>📋 Simple Form Validation 📋</h1>
<p>
    Welcome to the Simple Form Validation project! This web application provides a user-friendly form with real-time validation for name, email, and phone number inputs.
</p>
<br>
<h3>🚀 Features</h3>
<ul>
    <li>🛠 Real-time Validation: Ensures that all required fields are filled correctly before submission.</li>
    <li>🎨 Modern Design: Clean, intuitive interface with visually appealing elements.</li>
    <li>🔄 Error Handling: Provides immediate feedback on input errors to guide user corrections.</li>
</ul>
<br>
<h3>🔧 Technologies Used</h3>
<ul>
    <li>HTML: Structure and layout of the form.</li>
    <li>CSS: Styling and responsive design for a polished look.</li>
    <li>JavaScript: Functionality for form validation and user feedback.</li>
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
    &lt;form id="contactForm"&gt;: Defines the form with an ID of 'contactForm'.
        &lt;h2 class="contact-us"&gt;: A heading for the contact section.
        &lt;label for="name"&gt;: A label for the name input field.
        &lt;input type="text" id="name" name="name" required&gt;: An input field for entering the name.
        &lt;span id="nameError"&gt;: A container for displaying error messages for the name field.
        &lt;label for="email"&gt;: A label for the email input field.
        &lt;input type="email" id="email" name="email" required&gt;: An input field for entering the email.
        &lt;span id="emailError"&gt;: A container for displaying error messages for the email field.
        &lt;label for="phone"&gt;: A label for the phone input field.
        &lt;input type="tel" id="phone" name="phone"&gt;: An input field for entering the phone number.
        &lt;span id="phoneError"&gt;: A container for displaying error messages for the phone field.
        &lt;button type="submit"&gt;: A button to submit the form.
    &lt;/form&gt;
    &lt;script src="/js/main.js"&gt;&lt;/script&gt;: Links to an external JavaScript file that contains the logic for form validation.
&lt;/body&gt;
        </pre>
    </li>
    <li>
        <h4>CSS Styling</h4>
        <pre>
body: Styles the background and centers the content vertically and horizontally.
    background-image: url('/img/grunge-texture-4k-wallpapers.jpg'): Sets a full-screen background image.
    background-size: cover: Ensures the image covers the entire background area.
    background-position: center: Centers the background image.
    background-repeat: no-repeat: Prevents the background image from repeating.
form: Styles the form inside the container.
    background: #fff: Sets a white background for the form.
    padding: 40px: Adds padding inside the form.
    border-radius: 8px: Rounds the corners of the form.
    border: 5px solid #47B0AA: Adds a border around the form.
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1): Adds a subtle shadow for a 3D effect.
    max-width: 400px: Sets the maximum width of the form.
    width: 100%: Makes the form full-width within its container.
label: Styles the labels inside the form.
    display: block: Makes labels block-level elements.
    margin-bottom: 8px: Adds margin below labels.
    font-family: "Montserrat", sans-serif: Uses a sans-serif font.
    font-weight: 600: Uses semi-bold font weight.
    font-size: 16px: Sets the font size of labels.
    color: #47B0AA: Sets the color of label text.
input[type="text"],
input[type="email"],
input[type="tel"]: Styles the input fields inside the form.
    width: 100%: Makes input fields full-width.
    padding: 12px: Adds padding inside input fields.
    margin-bottom: 12px: Adds margin below input fields.
    border: 1px solid #47B0AA: Adds a border around input fields.
    border-radius: 4px: Rounds the corners of input fields.
    box-sizing: border-box: Ensures padding and border are included in the width and height.
    letter-spacing: 1.5px: Adds space between letters in input text.
    color: #239895: Sets the color of input text.
input::placeholder: Styles placeholder text in input fields.
    color: #888: Sets the default color for placeholder text.
input:not(:placeholder-shown): Styles input fields when placeholder is not shown.
    border-color: #47B0AA: Changes border color when input is filled.
input:-webkit-autofill: Styles input fields when autofilled by the browser.
    -webkit-box-shadow: 0 0 0 1000px white inset !important: Removes the default autofill background.
    -webkit-text-fill-color: #239895 !important: Sets the text color for autofilled fields.
button[type="submit"]: Styles the submit button.
    background-color: #47B0AA: Sets the background color of the button.
    color: white: Sets the text color of the button.
    border: none: Removes the default button border.
    padding: 10px 15px: Adds padding inside the button.
    border-radius: 4px: Rounds the corners of the button.
    cursor: pointer: Changes the cursor to a pointer on hover.
    font-family: "Montserrat", sans-serif: Uses a sans-serif font.
    font-weight: 600: Uses semi-bold font weight.
    font-size: 16px: Sets the font size of button text.
    transition: background-color 0.3s ease: Adds a transition effect for background color change on hover.
button[type="submit"]:hover: Styles the button when hovered over.
    background-color: #6AC9BE: Changes the button color on hover for a visual effect.
.error: Styles error messages.
    color: red: Sets the text color of error messages.
    font-size: 0.9em: Sets the font size of error messages.
    display: block: Makes error messages block-level elements.
    margin-top: 5px: Adds margin above error messages.
.contact-us: Styles the heading for the contact section.
    text-align: center: Centers the heading text.
    padding: 5px: Adds padding inside the heading.
    font-size: 30px: Sets the font size of the heading text.
    font-family: "Lora", serif: Uses a serif font for the heading text.
    font-weight: 400: Uses normal font weight for the heading text.
    margin-top: -12px: Adjusts the margin above the heading.
    text-transform: uppercase: Makes heading text uppercase.
    letter-spacing: 2px: Adds space between letters in the heading text.
    color: #47B0AA: Sets the color of the heading text.
.name, .email, .phone: Styles the input fields.
    font-family: "Montserrat", sans-serif: Uses a sans-serif font.
    font-weight: 600: Uses semi-bold font weight.
    font-size: 14px: Sets the font size of input text.
    color: #008080: Sets the color of input text.
        </pre>
    </li>
    <li>
        <h4>JavaScript Functionality</h4>
        <pre>
document.addEventListener("DOMContentLoaded", function() {
    const form = document.querySelector("form");
    const nameInput = document.getElementById("name");
    const emailInput = document.getElementById("email");
    const phoneInput = document.getElementById("phone");

    function validateForm(event) {
        event.preventDefault();
        const errors = document.querySelectorAll(".error");
        errors.forEach(error => error.textContent = '');

        let isValid = true;

        if (nameInput.value.trim() === '') {
            showError(nameInput, 'Name is required.');
            isValid = false;
        }

        if (emailInput.value.trim() === '') {


            showError(emailInput, 'Email is required.');
            isValid = false;
        } else if (!validateEmail(emailInput.value.trim())) {
            showError(emailInput, 'Email is invalid.');
            isValid = false;
        }

        if (phoneInput.value.trim() !== '' && !validatePhone(phoneInput.value.trim())) {
            showError(phoneInput, 'Phone number is invalid.');
            isValid = false;
        }

        if (isValid) {
            form.submit();
        }
    }

    function showError(input, message) {
        const errorSpan = document.getElementById(`${input.id}Error`);
        errorSpan.textContent = message;
    }

    function validateEmail(email) {
        const emailRegex = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
        return emailRegex.test(email);
    }

    function validatePhone(phone) {
        const phoneRegex = /^\d{10}$/;
        return phoneRegex.test(phone);
    }

    form.addEventListener("submit", validateForm);
});
        </pre>
    </li>
</ol>
