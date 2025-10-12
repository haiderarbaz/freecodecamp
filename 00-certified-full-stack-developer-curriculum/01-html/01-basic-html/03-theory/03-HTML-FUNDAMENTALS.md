# 🏷️ HTML Fundamentals

[⬅️ Back to BASICHTML.md](../BASICHTML.md)

This section covers the HTML Fundamentals like the div element, the id and class attributes, the HTML boilerplate, HTML entities, and more. You can explore the detailed documentation using the links below.

1. [What are Div Elements and When Should You Use Them?](https://www.freecodecamp.org/learn/full-stack-developer/lecture-html-fundamentals/what-are-div-elements)

2. [What Are IDs and Classes, and When Should You Use Them?](https://www.freecodecamp.org/learn/full-stack-developer/lecture-html-fundamentals/what-are-ids-and-classes)

3. [What Are HTML Entities, and What Are Some Common Examples?](https://www.freecodecamp.org/learn/full-stack-developer/lecture-html-fundamentals/what-are-html-entities)

4. [What Is the Role of the Script Element in HTML, and How Can It Be Used to Link to External JavaScript Files?](https://www.freecodecamp.org/learn/full-stack-developer/lecture-html-fundamentals/what-is-the-role-of-the-script-element-in-html)

---

## Short Summary from the above docs

This summary helps you quickly revise the key takeaways from the freeCodeCamp “HTML Fundamentals” docs.

---

## 📋 Table of Contents

- [📦 Div Elements](#📦-div-elements)
- [🆔 IDs and Classes](#🆔-ids-and-classes)
- [🔣 HTML Entities](#🔣-html-entities)
- [📜 Script Element](#📜-script-element)
- [🧠 Key Takeaways](#🧠-key-takeaways)

---

## 📦 Div Elements

**What are Div Elements and When Should You Use Them?**

- We are going to look at the Content Division Element - or in other words, the div:
  ```html
  <div></div>
  ```
- Think of the `div` as a beautiful being that can be anything you want it to be. You can give a `div` a `height`, we can give it a `width`, and you can give it a background color using CSS - or in other words styling.

- You can use it in a very basic form without styling to hold other elements together.

- For example, create a `div` and put a heading in it, and put a paragraph in it, and now these two elements will be grouped together:

  ```html
  <div>
    <h1>I am a heading</h1>
    <p>I am a paragraph</p>
  </div>
  ```

- Be aware that there might be better elements to use when grouping these together. You might choose a `section` element.

- For example:

  ```html
  <section>
    <h1>I am a heading</h1>
    <p>I am a paragraph</p>
  </section>
  ```

- This is because the `section` element has semantic meaning.

- Semantics are the meaning of words or phrases in a language.

- In HTML, which is a language, elements have their own semantic meaning too. So, this means if you use a `section` element, the browser will pick up its semantic meaning and understand to treat this as a section - on desktops, mobiles, you name it.

---

## 🆔 IDs and Classes

**What Are IDs and Classes, and When Should You Use Them?**

### IDs

- The `id` attribute adds a unique identifier to an HTML element.

- For example, there is an `h1` element with an `id` of `title`:

  ```html
  <h1 id="title">Movie Review Page</h1>
  ```

- You can reference the `id` name of `title` within your JavaScript or CSS.

- Below is a CSS example referencing the `id` of `title` to change the text `color` to `red`:

  ```css
  #title {
    color: red;
  }
  ```

  - The hash symbol `(#)` in front of `title`, tells the computer you want to target an `id` with that value.

- `id` names should not be used more than once, and they should always be unique.

- Another thing about `id` values, is that they cannot have spaces in them.

- Below is an example of applying the words `main` and `heading` to an `id` attribute value:

  ```html
  <h1 id="main heading">Main heading</h1>
  ```

  - Browsers will see this space as part of the `id` which will lead to unwanted issues when it comes to styling and scripting.

- `id` attribute values should only contain letters, digits, underscores, and dashes.

### Classes

- The `class` attribute value does not need to be unique and can contain spaces.

- Below is an example of applying a class called `box` to a `div` element:
  ```html
  <div class="box"></div>
  ```
- If you want to add multiple class names to an element, you can do so by separating the names by a space.

- Below is an updated example applying multiple classes to a `div` element:

  ```html
  <div class="box red-top"></div>
  ```

- To apply a set of styles to that box class, you can reference that class inside your CSS.

- Below is an example of setting width, height, and border properties to the element with the class name of box:

  ```css
  .box {
    width: 200px;
    height: 200px;
    border: 2px solid black;
  }
  ```

  - The dot symbol (.) in front of box, tells the computer you want to target a class with that value.

- When the code runs, it will search through all of your HTML document to find all elements with that class name and apply those styles.

**Note:**

- Classes are best used when you want to apply a set of styles to many elements.
- If you want to target a specific element, it is best to use id because those values need to be unique.

---

## 🔣 HTML Entities

**What Are HTML Entities, and What Are Some Common Examples?**

- An HTML entity, or character reference, is a set of characters used to represent a reserved character in HTML.

- For example, there is a paragraph element with an image element nested inside:

  ```html
  <p>This is an <img /> element</p>
  ```

- The text on the screen should say `This is an <img/> element`. However, the text currently says `This is an element`.
- This is happening because when the HTML parser sees the less than `(<)` symbol followed by an HTML tag name, it interprets that as an HTML element.

- To fix this issue, you can use HTML entities.

- Below is an updated example using the correct HTML entities for the less than and greater than `(>)` symbols.

  ```html
  <p>This is an &lt;img /&gt; element</p>
  ```

- These types of character references are known as named character references. Named references start with an ampersand sign `(&)` and end with a semicolon `(;)`.

- By using a named character reference, the HTML parser will not confuse this with an actual HTML element.

- Here is what the updated paragraph element looks like on the page: `This is an <img/> element`. Now, users will be able to see the entire image element syntax as you intended it.

- Another type of character reference would be the decimal numeric reference.

- Below is an example of using the decimal numeric reference for the less than symbol:

  ```html
  &#60;
  ```

  - This character reference starts with an ampersand sign and hash symbol `(#)`, followed by one or more decimal digits, followed by a semicolon.

- The last type of character reference would be the hexadecimal numeric reference.

- Below is an example of using the hexadecimal numeric reference for the less than symbol:

  ```html
  &#x3C;
  ```

  - This character reference starts with an ampersand sign, hash symbol, and the letter x. Then it is followed by one or more ASCII hex digits and ends with a semicolon.

- Some other examples of using HTML entities, you often see them used for symbols like the copyright symbol `(©)`, quotes `(")`, trademark symbol `(™)`, and the ampersand sign.

---

## 📜 Script Element

**What Is the Role of the Script Element in HTML, and How Can It Be Used to Link to External JavaScript Files?**

- The `script` element is used to embed executable code.

- You will use this to execute JavaScript code.

- JavaScript is used to add interactivity to your web pages.

- Common examples of using JavaScript include interactive games, image sliders, and dynamic forms that validate user input in real-time.

- Below is an example of using the `script` element in an HTML document:

  ```html
  <body>
    <script>
      alert("Welcome to freeCodeCamp");
    </script>
  </body>
  ```

  - In this example, we have an `alert` to display the message `Welcome to freeCodeCamp`.
  - When the page first loads, the alert will pop up. Then the user can click on the OK button to dismiss the message.

- You can technically write all of your JavaScript code inside the script tags, but it is considered best practice to link to an external JavaScript file instead.

- Below is an example of using the script element to link to an external JavaScript file:

  ```html
  <script src="path-to-javascript-file.js"></script>
  ```

  - The `src` attribute is used here to specify the location for that external JavaScript file.

  - `src` stands for "source".

  - The reason why it is not encouraged to place all of your JavaScript inside the HTML document is because of separation of concerns.

  - Separation of concerns is a design principle where you separate your programs into distinct sections and have each section address a separate concern.

  - In this case, we want to separate our JavaScript code from our HTML code.

---

## 🧠 Key Takeaways

- Divs are generic containers for grouping content
- IDs must be unique; classes can be reused
- HTML entities represent reserved characters
- Script elements link JavaScript to your HTML
