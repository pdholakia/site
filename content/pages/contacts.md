---
title: "Contact me"
template: "page"
---

<style type="text/css">
body {
  font-family: 'Lato', georgia;
  font-size: 25px;
  /*color: rgba(100, 100, 100, 1);*/
  /*background: linear-gradient(90deg, #ee5c87, #f1a4b5, #d587b3);*/
  font-weight: 300;
  -webkit-font-smoothing: antialiased;
}

#contact-form {
  max-width: 90%;
  margin: 0 auto;
  text-align: center;
}

label {
  font-weight: 400;
  cursor: pointer;
}

textarea,
input {
  border: none;
  outline: none;
  border-radius: 0;
  text-align: center;
  background: none;
  font-weight: 700;
  font-family: 'Lato', georgia;
  font-size: 25px;
  color: rgba(100, 100, 100, 1);
  max-width: 90%;
  padding: 1rem;
  border: 2px dashed rgba(100, 100, 100, 0);
  box-sizing: border-box;
  cursor: text;
}

textarea {
  text-align: left;
  /* overflow:hidden; */ 
  resize: none;
  width: 90%;
  border-color: rgba(100, 100, 100, 0)
}
/* Learn about this code on MDN: https://developer.mozilla.org/en-US/docs/Web/CSS/%3Afocus */
textarea:focus {
  background-color: rgba(100, 100, 100, 0.2);
  border: 2px dashed rgba(100, 100, 100, 1);
}
/* Learn about this code on MDN:  https://developer.mozilla.org/en-US/docs/Web/CSS/:required */
textarea:focus:required:valid {
  border: 2px solid rgba(100, 100, 100, 0);
  border-bottom: 2px solid rgba(100, 100, 100, 0.2);
}
/* Learn about this code on MDN:  https://developer.mozilla.org/en-US/docs/Web/CSS/:valid */
textarea:required:valid {
  border-bottom: 2px solid rgba(100, 100, 100, 0.2);
}

input {
  border-bottom: 2px dashed rgba(100, 100, 100, 0.5);
}

input:required,
textarea:required {
  border-bottom: 2px dashed rgba(100, 100, 100, 0.5);
}

input:focus {
  border-bottom: 2px dashed rgba(100, 100, 100, 1);
  background-color: rgba(100, 100, 100, 0.2);
}

input:required:valid {
  border-bottom: 2px solid rgba(100, 100, 100, 0.2);
}
/* Learn about this code on MDN: https://developer.mozilla.org/en-US/docs/Web/CSS/:invalid */
input:required:invalid {
  color: rgba(100, 100, 100, 0.5);
}
/* Selecting placeholder with pseudo-classes is only supported in newest browsers */ 
[placeholder] {
  text-align: center;
  color: rgba(100, 100, 100, 0.4);
  font-style: italic;
  font-weight: 400;
}
::-webkit-input-placeholder {
  text-align: center;
  color: rgba(100, 100, 100, 0.4);
  font-style: italic;
  font-weight: 400;
}

::-moz-placeholder {
  /* Firefox 19+ */  
  text-align: center;
  color: rgba(100, 100, 100, 0.4);
  font-style: italic;
  font-weight: 400;
}

:-ms-input-placeholder {
  text-align: center;
  color: rgba(100, 100, 100, 0.4);
  font-style: italic;
  font-weight: 400;
}

/* :checked */
input[type="checkbox"]{
   cursor: pointer;
   width: 30px; height: 30px;
   vertical-align: middle;
   outline: none;
}
:checked + label {
    padding: .5em;
    color: rgba(236, 181, 62, 0.95);
    background-color: rgba(100, 100, 100, 1);
    transition: .3s;
}
/* Learn about this code on MDN: https://developer.mozilla.org/en-US/docs/Web/CSS/:in-range */
input:in-range {
    color: rgba(236, 181, 62, 0.95);
    background-color: rgba(100, 100, 100, 1);  
}
input:out-of-range {
   color: rgba(100, 100, 100, 0.4);  
}
input:in-range + label::after {
    content: 'OK';
}
input:out-of-range + label::after {
    content: 'out of range!';
}
/* textarea */
.expanding {
  vertical-align: top;
}

.send {
  fill: rgba(100, 100, 100, 1)
}

.send:hover {
  fill: rgba(0, 0, 0, 1);
  cursor: pointer;
}

button {
  background: none;
  border: none;
  outline: none;
  margin: 2%;
}

button:hover small {
  opacity: 1;
}

small {
  display: block;
  opacity: .5;
  margin-bottom: 1%;
}

.tutorial {
  opacity: 1;
  font-size: 16px;
  color: white;
  position: relative;
  text-align: center;
  display: block;
  margin-top: 7%;
  
}

.tutorial a {
  color: white;
}
/* Based on a lovely design by @Erlen */
</style>

<link href='https://fonts.googleapis.com/css?family=Lato' rel='stylesheet' type='text/css'>

<!--HTML 5 Form-->
<form id="contact-form" action="" name="contact" method="post" data-netlify="true" data-netlify-honeypot="bot-field">
  <input type="hidden" name="bot-field" />
  <input type="hidden" name="form-name" value="contact" />
  <p>Hi!</p>
  <p>My
    <label for="your-name">name</label> is
    <input type="text" name="your-name" id="your-name" minlength="2" placeholder="(your name here)" required> and</p>

  <p>my
    <label for="email">email address</label> is
    <input type="email" name="your-email" id="email" placeholder="(your email address)" required>
  </p>

  <p> I have a
    <label for="your-message">message</label> for you,</p>

  <p>
    <textarea name="your-message" id="your-message" placeholder="(your msg here)" class="expanding" required></textarea>
  </p>

  <p>
    <button type="submit" value="send">
      <svg version="1.1" class="send" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" x="0px" y="0px" width="100px" height="36px" viewBox="0 0 100 36" enable-background="new 0 0 100 36" xml:space="preserve">
        <path d="M100,0L100,0 M23.8,7.1L100,0L40.9,36l-4.7-7.5L22,34.8l-4-11L0,30.5L16.4,8.7l5.4,15L23,7L23.8,7.1z M16.8,20.4l-1.5-4.3
	l-5.1,6.7L16.8,20.4z M34.4,25.4l-8.1-13.1L25,29.6L34.4,25.4z M35.2,13.2l8.1,13.1L70,9.9L35.2,13.2z" />
      </svg>
    </button>
  </p>
</form>
