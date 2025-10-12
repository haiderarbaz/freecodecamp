# 🏷️ Understanding the HTML Boilerplate

[⬅️ Back to BASICHTML.md](../BASICHTML.md)

This section covers the HTML boilerplate which is a ready-made template for your webpages. You will learn how to work with the link element, meta element and more. You can explore the detailed documentation using the links below.

1. [What Is the Role of the Link Element in HTML, and How Can It Be Used to Link to External Stylesheets?](https://www.freecodecamp.org/learn/full-stack-developer/lecture-understanding-the-html-boilerplate/what-is-the-role-of-the-link-element-in-html)

2. [What Is an HTML Boilerplate, and Why Is It Important?](https://www.freecodecamp.org/learn/full-stack-developer/lecture-understanding-the-html-boilerplate/what-is-an-html-boilerplate)

3. [What Is UTF-8 Character Encoding, and Why Is It Needed?](https://www.freecodecamp.org/learn/full-stack-developer/lecture-understanding-the-html-boilerplate/what-is-utf-8-character-encoding)

---

## Short Summary from the above docs

This summary helps you quickly revise the key takeaways from the freeCodeCamp “Understanding the HTML Boilerplate” docs.

---

## 📋 Table of Contents

- [🔗 Link](#🔗-link)
- [📄 HTML Boilerplate](#📄-html-boilerplate)
- [🔡 UTF-8 Character Encoding](#🔡-utf-8-character-encoding)

---

## 🔗 Link

- The `link` element is used to link to external resources like stylesheets and site icons.
- Here is the basic syntax for using the `link` element for an external CSS file:

  ```html
  <link rel="stylesheet" href="./styles.css" />
  ```

  - The `rel` attribute is used to specify the relationship between the linked resource and the HTML document.
  - In this situation, we need to specify that this linked resource is a `stylesheet`.
  - The `href` attribute is used to specify the location of the URL for the external resource.
  - The `dot` followed by a forward slash in the example tells the computer to look in the current folder, or directory, for the `styles.css` file.

- It is considered best practice to separate your HTML and CSS in different files.
- You will use the `link` element for your external CSS file instead of writing everything in the HTML document.

- The `link` element should be placed inside the `head` element as seen in the following example:

  ```html
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Examples of the link element</title>
    <link rel="stylesheet" href="./styles.css" />
  </head>
  ```

- Sometimes you will see multiple `link` elements inside a professional codebase that link to different stylesheets, fonts, and icons.

- Here is an example of using the `link` element to link to an external Google Font called Playwright Cuba:

  ```html
  <link rel="preconnect" href="https://fonts.googleapis.com" />
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
  <link
    href="https://fonts.googleapis.com/css2?family=Playwrite+CU:wght@100..400&display=swap"
    rel="stylesheet"
  />
  ```

  - In the above code example, the `preconnect` value for the `rel` attribute tells the browser to create an early connection to the value specified in the `href` attribute.
  - This is done to speed up loading times for these external resources.

- Google Fonts are a set of free and open source custom fonts that you can use inside any project. You can choose which fonts you would like to use and Google will provide you with the necessary HTML and CSS code.

- Another common use case for the `link` element is to link to icons.

- Here is an example of linking to a favicon:

  ```html
  <link rel="icon" href="favicon.ico" />
  ```

- A favicon, which is short for favorite icon, is a small icon typically displayed in the browser tab next to the site title. A lot of websites will use a favicon to display their brand icon.

---

## 📄 HTML Boilerplate

- **What is the HTML boilerplate?**
- It's like a ready-made template for your webpages
- It includes the basic structure and essential elements every HTML document needs.
- It saves your time and helps ensure your pages are set up properly.

- Here is an example:

  ```html
  <!DOCTYPE html>
  <html lang="en">
    <head>
      <meta charset="utf-8" />
      <meta name="viewport" content="width=device-width, initial-scale=1.0" />
      <title>freeCodeCamp</title>
      <link rel="stylesheet" href="./styles.css" />
    </head>
    <body></body>
  </html>
  ```

- Think of it as the foundations of a house.

- The key parts of the boilerplate.

  1.  First, the `DOCTYPE` declaration:

      ```html
      <!DOCTYPE html>
      ```

      - It tells the browsers which version of HTML you're using.

  2.  Second, the `html` tag:

      ```html
      <!DOCTYPE html>
      <html lang="en">
        <!--All other elements go inside here-->
      </html>
      ```

      - This wraps around all your content, and can specify the language of your page.

  3.  Inside the `html` tag, you'll find two main sections - a `head`, and a `body`:

      ```html
      <!DOCTYPE html>
      <html lang="en">
        <head>
          <!--Important metadata goes here-->
        </head>
        <body>
          <!--Headings, paragraphs, images, etc. go inside here-->
        </body>
      </html>
      ```

      - The `head` section contains important behind-the-scenes information:

        ```html
        <head>
          <meta charset="UTF-8" />
          <meta
            name="viewport"
            content="width=device-width, initial-scale=1.0"
          />
          <title>Document Title Goes Here</title>
          <link rel="stylesheet" href="./styles.css" />
        </head>
        ```

        - Your site's metadata, contained in `meta` elements, has details about things like character encoding, and how websites like Twitter should preview your page's link.
        - Your site's title, found in the `title` element, determines the text that appears in the browser tab or window.
        - Finally, you'll typically link your page's external stylesheets in the `head` section using `link` elements.

      - The `body` section is where all your content goes:

        ```html
        <body>
          <h1>I am a main title</h1>
          <p>Example paragraph text</p>
        </body>
        ```

- **Why is the boilerplate important?**
- It ensures your pages are structured correctly and work well across different browsers.
- Using a boilerplate helps you avoid common mistakes and follow best practices.
- It's a great starting point for any web project.

---

## 🔡 UTF-8 Character Encoding

- **What is UTF-8 character encoding, and why is it needed?**

- UTF-8 (UCS Transformation Format 8) is the most common character encoding used on the web. It's the system that allows computers to store and display text.

- How it works:

  - All text you see on a webpage is stored as data (bytes)

  - A byte is a unit of data made up of 8 bits (binary digits)

  - `UTF-8` translates characters into this byte format so computers can read them

- Why `UTF-8` is important:

  - It supports every character from the Unicode character set
  - This includes all languages, symbols, emojis, and technical characters worldwide
  - It's the universal standard that makes the web accessible in any language

- `UTF-8` is like a universal translator that lets computers understand and display any character from any language or symbol system.

- Here is an example of using the `meta` element with the `charset` attribute to set the character encoding to UTF-8:

  ```html
  <meta charset="UTF-8" />
  ```

  - By setting the character encoding to UTF-8, it will ensure that the accented `"e"` character `(é)` is displayed correctly on the page.

- Here is an extended code example of using the UTF-8 character encoding:

  ```html
  <!DOCTYPE html>
  <html lang="en">
    <head>
      <meta charset="UTF-8" />
      <meta name="viewport" content="width=device-width, initial-scale=1.0" />
      <title>Examples of the UTF-8 encoding</title>
    </head>
    <body>
      <p>Café</p>
    </body>
  </html>
  ```

- For each new project you create, you should include this `meta` element with the `charset` attribute set to `UTF-8`.
