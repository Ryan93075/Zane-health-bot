DOCUMENTATION:

<The helth bot works with the help of OpenAI API>

The primary objective of this project is to enhance its capability by incorporating comprehensive user health history information and advanced analytics. By leveraging this enriched data, we aim to deliver highly accurate and reliable results. Our goal is to provide world-class medical support that is accessible to individuals from all walks of life. We are confident in our ability to achieve this vision and empower even the average person with exceptional healthcare solutions. 


The index.html and all supporting files are places inside /root.

INDEX.HTML:

Document Structure


<!DOCTYPE html>: Specifies that the document is an HTML5 document.

<html lang="en-US" dir="ltr">: Defines the root element of the HTML document. lang attribute specifies the language and dir attribute specifies the text direction.

Head Section:

<head>: Contains metadata and other information about the HTML document.
Inside the <head> section:

<meta charset="utf-8">: Specifies the character encoding for the HTML document.
<meta http-equiv="X-UA-Compatible" content="IE=edge">: Instructs Internet Explorer to use the latest rendering engine.

<meta name="viewport" content="width=device-width, initial-scale=1">: Sets the viewport width and initial scale for responsive layouts.

Title: <title>Livedoc | Landing, Responsive &amp; Business Templatee</title>: Sets the title of the document shown in the browser's title bar.

Favicon: Various <link> tags specify different favicon images for different platforms.
Stylesheets:

<link href="assets/css/theme.css" rel="stylesheet" />: Links the CSS file "theme.css" to the HTML document.

Body Section:

<body>: Contains the visible content of the HTML document.

Inside the <body> section:

CSS Styling: Sets CSS rules to define the styles for the body, background container, and buttons.
<div class="background-container">: Creates a container for the background video or iframe.
<iframe>: Embeds a Sketchfab model as an iframe, which can be interacted with on the webpage.
Additional CSS Styling: Sets CSS rules for the glowing button, link, and text centering.
<main>: Defines the main content section of the webpage.
<nav>: Creates a navigation bar with links to different sections of the webpage.
<section>: Represents a section of the webpage.
Content: Contains headings, paragraphs, and buttons for different sections of the webpage.

<section class="py-5">: Represents a section of the webpage with padding on the top and bottom.

Background Image: Sets a background image for the section using the background-image property.

<div class="container">: Creates a container for the content within the section.

<div class="row align-items-center">: Creates a row with vertically centered content.

<div class="col-md-6 order-lg-1 mb-5 mb-lg-0">: Creates a column for the image on medium-sized screens, with a specified order.

<img class="fit-cover rounded-circle w-100" src="assets/img/gallery/health-care.png" alt="..." />: Displays an image that fits the container with rounded corners.

<div class="col-md-6 text-center text-md-start">: Creates a column for text content on medium-sized screens, with different alignment based on the screen size.

Content: Contains headings, paragraphs, and a button.

<section class="pb-0">: Represents a section of the webpage with padding at the bottom.

<div class="container">: Creates a container for the content within the section.

<div class="row">: Creates a row to hold the content.

<div class="col-12 py-3">: Creates a column for the content, with padding on the top and bottom.

Background Image: Sets a background image for the section using the background-image property.

<h1 class="text-center">OUR CREATORS</h1>: Displays a heading centered on the page.

<section class="py-5">: Represents a section of the webpage with padding on the top and bottom.

Background Image: Sets a background image for the section using the background-image property.

<div class="container">: Creates a container for the content within the section.

<div class="row flex-center">: Creates a row with horizontally centered content.

<div class="col-xl-10 px-0">: Creates a column that spans the entire width of extra-large screens, with no padding.

Carousel: Creates a carousel to display multiple items.

Carousel Items: Contains multiple carousel items with images, headings, paragraphs, and buttons.

<section class="py-5">: Represents a section of the webpage with padding on the top and bottom.

<div class="container">: Creates a container for the content within the section.

<div class="row">: Creates a row to hold the content.

<div class="col-12 py-3">: Creates a column for the content, with padding on the top and bottom.

Background Image: Sets a background image for the section using the background-image property.

<h1 class="text-center">REGISTER HERE</h1>: Displays a heading centered on the page.

<section class="py-8">: Represents a section of the webpage with larger padding on the top and bottom.

<div class="container">: Creates a container for the content within the section.

<div class="row">: Creates a row to hold the content.

<div class="bg-holder bg-size" style="background-image:url(assets/img/gallery/dot-bg.png);background-position:bottom right;background-size:auto;">: Sets a background image for the section using the background-image property.

<div class="col-lg-6 z-index-2 mb-5">: Creates a column for the image on large screens.

<img class="w-100" src="assets/img/gallery/appointment.png" alt="..." />: Displays an image that spans the entire column width.

<div class="col-lg-6 z-index-2">: Creates a column for the form on large screens.

Form: Contains a form with input fields, a select dropdown, a textarea, and a button.

<section class="py-5">: Represents a section of the webpage with padding on the top and bottom.

<div class="container">: Creates a container for the content within the section.

<div class="row">: Creates a row to hold the content.

<div class="col-12 py-3">: Creates a column for the content, with padding on the top and bottom.

Background Image: Sets a background image for the section using the background-image property.

<h1 class="text-center">RECENT BLOGPOSTS</h1>: Displays a heading centered on the page.

<section>: Represents a section of the webpage.

Background Image: Sets a background image for the section using the background-image property.

<div class="container">: Creates a container for the content within the section.

<div class="row">: Creates a row to hold the content.

Cards: Contains multiple cards with images, headings, and links.


STYLE.CSS(for bot):

*: Applies the following styles to all elements on the page.

body: Sets the background color of the body.

.chatbot-toggler: Styles the chatbot toggler button, which is a circular button displayed on the bottom right of the page.

.chatbot-toggler span: Styles the text inside the chatbot toggler button.

.chatbot: Styles the chatbot container.

.chatbot header: Styles the header section of the chatbot.

.chatbot header span: Styles the close button in the chatbot header.

.chatbot .chatbox: Styles the chatbox container.

.chatbox .chat: Styles the individual chat messages.

.chatbox .outgoing: Styles the outgoing chat messages.

.chatbox .incoming span: Styles the avatar icon for incoming chat messages.

.chatbox .chat p: Styles the chat message content.

.chatbox .chat p.error: Styles the error message content.

.chatbot .chat-input: Styles the chat input container.

.chat-input textarea: Styles the textarea for user input.

.chat-input span: Styles the send button for user input.

Media query @media (max-width: 490px): Contains responsive styles for screens with a maximum width of 490 pixels.	

SCRIPT.JS(script for bot):

The script starts by selecting various elements from the HTML using document.querySelector() and assigning them to variables.

The createChatLi() function creates a chat message <li> element with the passed message and className (either "outgoing" or "incoming").

The generateResponse() function sends a POST request to the OpenAI API to generate a response based on the user's message. It retrieves the response and sets it as the text content of the chat message.

The handleChat() function is called when the user sends a chat message. It retrieves the user's message, clears the input textarea, and appends the user's message to the chatbox. It then calls generateResponse() to generate and display the response message.

Event listeners are added to the input textarea and send button. The input event listener adjusts the height of the input textarea based on its content. The keydown event listener checks if the Enter key is pressed without the Shift key, and if so, it calls handleChat() to handle the chat. The send button click event listener also calls handleChat() to handle the chat.

Additional event listeners are added to the close button and chatbot toggler button to show/hide the chatbot component.

Note: The script includes a placeholder value PASTE-YOUR-API-KEY for the API_KEY constant. You need to replace it with your actual OpenAI API key to make the chatbot work with OpenAI's GPT-3.5 Turbo model.

Make sure to replace PASTE-YOUR-API-KEY with your OpenAI API key and integrate the chatbot HTML, CSS, and JavaScript code properly in your project for the chatbot functionality to work.

EXPECTED ERROR(Expired API key):

Additional keys are given in keys.txt