# 🏷️ Understanding HTML Attributes

[⬅️Back to BASICHTML.md](../BASICHTML.md)

This section covers the theory behind HTML attributes. You can explore the detailed documentation using the links below.

1. [What Role Does HTML Play on the Web?](https://www.freecodecamp.org/learn/full-stack-developer/lecture-understanding-html-attributes/what-is-html)

2. [What Are Attributes, and How Do They Work?](https://www.freecodecamp.org/learn/full-stack-developer/lecture-understanding-html-attributes/what-are-attributes)

---

## Short Summary from the above docs

This summary helps you quickly revise the key takeaways from the freeCodeCamp “Understanding HTML Attributes” docs.

- HTML, which stands for HyperText Markup Language, is a markup language for creating web pages.

  - When you visit a website and see content like paragraphs, headings, links, images, and videos, that's HTML.
  - It's the code that defines the structure and content of a webpage through the use of elements; HTML is made up of these elements.

  - Here's an example of a paragraph element:

    ```html
    <p>Hello</p>
    ```

  - The first one you will use is the h1 element:

    ```html
    <h1>Welcome to freeCodeCamp</h1>
    ```

  - It starts with an opening tag (`<h1>`) and ends with a closing tag (`</h1>`), displaying the text in between.

- Most elements will have an opening tag and a closing tag. Sometimes those tags are referred to as start and end tags.
- In between those two tags, you will have the content.
- This content can be text or other HTML elements.
- Both opening and closing tags start with a left angle bracket (`<`), and end with a right angle bracket (`>`), with the tag name placed between these angle brackets.
- While HTML tag names are case-insensitive, it is a widely accepted convention and best practice to write them in lowercase.
- Here is a closer look at just the opening and closing paragraph tags:

  ```html
  <p></p>
  ```

- What distinguishes an opening tag from a closing tag is the forward slash (`/`) placed immediately after the left angle bracket in a closing tag.

- An `h1` element is the main heading of a webpage, and you should only use one per page.
- `h2` elements represent subheadings.
- You can have multiple per page, and they look like this:

  ```html
  <h2>This is a subheading.</h2>
  ```

- When you need to add a paragraph to a webpage, you can use the p element like this:

  ```html
  <p>This is a paragraph element.</p>
  ```

- There are six heading elements in HTML: h1 through h6.
- They're used to show the importance of sections on your webpage, with h1 being the most important and h6 the least.

- Some HTML elements do not have a closing tag. These are known as void elements.
- Here is an example of an image element, which is a void element:

  `<img>`

- While many code formatters like Prettier will choose to include the `/` in void elements, the HTML spec states that the presence of the `/` "does not mark the start tag as self-closing but instead is unnecessary and has no effect of any kind".

- If you wanted to display an image, you will need to include a couple of attributes inside your image element.

- An attribute is a special value used to adjust the behavior for an HTML element

  ```html
  <img src="image location" />
  ```

  - The src attribute is used to specify the location for that image.
  - For image elements, it's good practice to include another attribute called the alt attribute.
  - Here's an example of an image element with the src and alt attributes:

    ```html
    <img src="example-cat-img-url" alt="Cat sleeping in the grass" />
    ```

  - The alt attribute is used to provide short, descriptive text for the images.
  - In this case, the descriptive text is "Cat sleeping in the grass".

---

### What Are Attributes, and How Do They Work?

- An attribute is a value placed inside the opening tag of an HTML element.
- Attributes provide additional information about the element or specify how the element should behave.

- Here is the basic syntax for an attribute:

  ```html
  <element attribute="value"></element>
  ```

  - The value can be a string or a number, depending on the attribute.

- The first example is the `href` attribute, which is used to specify the URL of a link:

  ```html
  <a href="https://www.example-website.com">Visit our website</a>
  ```

  - Without this attribute, the link would not work because there would be no destination URL.
  - So you must include this `href` attribute to make the link functional.

- Some common attributes are the `src`, or source, and `alt`, or alternative, attribute, which is used to specify the source of an image and provide alternative descriptive text for the image, respectively:

  ```html
  <img src="image.jpg" alt="A beautiful image" />
  ```

- Similar to the `href` attribute, the `src` attribute is required because it specifies the image file to be displayed.
- The `alt` attribute is not required, but it is recommended for `accessibility` purposes.
- `Accessibility` means making sure that everyone, including those with disabilities, can use and understand things like websites, apps, and physical spaces.

- Some attributes are a little unique with their syntax, like the `checked` attribute shown here:

  ```html
  <input type="checkbox" checked />
  ```

  - In the following example, we have an input element with the `type` attribute set to `checkbox`.
  - `Inputs` are used to collect data from users, and the `type` attribute specifies the type of `input`.
  - In this case, this input is a `checkbox`.
  - The `checked` attribute is used to specify that the `checkbox` should be `checked` by default.
  - The `checked` attribute does not require a value.
  - If it is present, the `checkbox` will be `checked` by default.
  - If the attribute is not present, the checkbox will be unchecked. This is known as a `Boolean attribute`.

- There are several common `Boolean attributes` you will encounter in HTML, such as disabled, readonly, and required.
- These attributes are used to specify the state of an element, such as whether it is disabled, read-only, or required.

- HTML has many attributes that can be used to customise the behaviour and appearance of elements on a webpage.
- Understanding how to use attributes is essential for creating interactive and accessible web content.

- While **HTML** defines the structure and content of a webpage, **CSS** is used to add style — things like colors, fonts, spacing, and layout.

- Finally, **JavaScript** makes your webpage interactive — it lets you tell the page what to do when someone clicks a button, submits a form, or many other things.

- **HTML** is for the content and structure. **CSS** is for styling. **JavaScript** is for adding interactivity to your web pages.
  - A good analogy for this is to compare HTML, CSS, and JavaScript with a complete building.
    - **HTML** represents the blocks, concrete, and irons that make up the walls. It's the foundation that makes the building strong.
    - **CSS** represents the interior and exterior design that makes the house look beautiful.
    - **JavaScript** represents the electrical and water system that ensures uninterrupted access to water and electricity.

---

## 🧠 Key Takeaway:

Attributes define additional information or behavior for HTML elements.  
Understanding them is essential to building structured, accessible, and interactive web pages.
