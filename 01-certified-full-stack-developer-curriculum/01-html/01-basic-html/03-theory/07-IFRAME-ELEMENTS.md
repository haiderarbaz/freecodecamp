# 🏷️ Working with the iframe Element

[⬅️ Back to BASICHTML.md](../BASICHTML.md)

In this section, you will learn how to work with the iframe element which is used to embed an external site on your web page.

1. [What Are Replaced Elements, and What Are Some Examples?](https://www.freecodecamp.org/learn/full-stack-developer/lecture-working-with-media/what-are-replaced-elements)

2. [How Do You Embed Videos onto Your Page Using the iframe Element?](https://www.freecodecamp.org/learn/full-stack-developer/lecture-working-with-media/how-do-you-embed-videos-onto-your-page-using-the-iframe-element)

---

## Short Summary from the above docs

This summary helps you quickly revise the key takeaways from the freeCodeCamp “Working with the iframe Element" docs.

---

## 📋 Table of Contents

- [🔄 Replaced Elements](#🔄-replaced-elements)
- [🖼️ iframe Element](#🖼️-iframe-element)
- [🧠 Key Takeaways](#🧠-key-takeaways)

---

## 🔄 Replaced Elements

- A `replaced element` is an element whose content is determined by an external resource rather than by CSS itself. CSS, or cascading stylesheets, is used to add styles to a web page.

- Common examples of `replaced elements` include the `image`, `iframe`, and `video` elements.

- With replaced elements, you can control the position, or layout of an element.

- But your CSS cannot directly modify the content of that element.

- This might be easier to explain with some examples.

- Consider the image element, which embeds an image on your web page:

  ```html
  <img src="example-img-url" alt="Descriptive text goes here" />
  ```

- The element itself is replaced with the external object: the image.

- Your CSS can control things like the positioning of the image, or apply a filter to it, but you cannot actually modify the image itself.

- A more robust example might be the `iframe` element, which embeds an external site on your web page.

- Below is an example of using the `iframe` element for a popular YouTube video on the freeCodeCamp channel.

  ```html
  <iframe
    width="400"
    height="200"
    src="https://www.youtube.com/embed/u43gJJrVa1I?si=BoDW_puFsy8OEr_Z"
    title="Professional Cloud Architect Certification Course – Pass the Exam! (YouTube video)"
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
    referrerpolicy="strict-origin-when-cross-origin"
    allowfullscreen
  ></iframe>
  ```

  - Allow attributes is like a permission list that tells the browser what features the iframe is allowed to use.
  - In the `allow` attribute
    - `accelerometer` lets the iframe use motion sensors so it can detect things like device tilting and rotation.
    - `autoplay` lets the video start playing automatically, and
    - `clipboard-write` lets the iframe write data to the user’s clipboard.
    - `encrypted-media`, `gyroscope`, and `web-share` will allow the use of encrypted media extensions to protect the video, let the iframe pop out into `picture-in-picture` mode when needed, and allow sharing the iframe content through the device's native share dialogs.
    - `referrerpolicy`, it is the rule that determines how much detail you share when your page connects to another page.
    - `allowfullscreen` attribute allows the user to display the `iframe` in full screen mode.

- If you want to see different videos in the preview window, change the value of the `src` attribute to a video of your choosing.

- **NOTE:** Don't worry about the extra attributes mentioned in the interactive example like `referrerpolicy` and `allowfullscreen`. You will learn more about working with `iframe` elements in a
  future workshop.

- Other common examples of using the `iframe` element would be to embed maps onto the page.
- Below is an example of an embedded map.

  ```html
  <iframe
    title="Map of the Royal Observatory, Greenwich, London"
    width="300"
    height="200"
    src="https://www.openstreetmap.org/export/embed.html?bbox=-0.004017949104309083%2C51.47612752641776%2C0.00030577182769775396%2C51.478569861898606&amp;layer=mapnik"
  >
  </iframe>
  ```

**_Try playing around with the map itself by zooming in/out_**

- The element itself is replaced with the external object: the site.

- Your CSS can change the positioning of the embedded site, but you cannot modify the site's contents.

- To dive a bit further, if the embedded site has an h1 element, your CSS would not be able to style that h1 element. You cannot change the size, font color, and so on.

- There are some other replaced elements, such as video, and embed. And some elements behave as replaced elements under specific circumstances.

- Below is an example of an input element with the type attribute set to image:

  ```html
  <input type="image" alt="Descriptive text goes here" src="example-img-url" />
  ```

  - This type of input is considered to be a replaced element, but other input types like text, or email are not replaced elements.

---

## 🖼️ iframe Element

- This element stands for inline frame.

- It's an inline element used to embed other HTML content directly within the HTML page. That HTML content could be a video, map, another HTML element, or even other web pages.

- Below is an example of embedding a popular freeCodeCamp course from YouTube.

  ```html
  <iframe
    width="400"
    height="400"
    src="https://www.youtube.com/embed/PkZNo7MFNFg?si=-UBVIUNM3csdeiWF"
    title="Learn JavaScript - Full Course for Beginners (YouTube video)"
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
    referrerpolicy="strict-origin-when-cross-origin"
    allowfullscreen
  ></iframe>
  ```

  - To see a different video, change the src value to a video of your choosing.

  - The `src` attribute specifies the URL of the page you want to embed.
  - The `width` attribute specifies the width of the `iframe`.
  - The `height` attribute specifies the height of the `iframe`.
  - The `allowfullscreen` attribute allows the user to display the `iframe` in full screen mode.
  - It's also a good practice to specify a `title` attribute for the `iframe`, as it's important for accessibility.

- **Note:** The video can come from anywhere. It doesn't have to come from video services like YouTube and Vimeo.

- Don't forget you can also embed a map, another web page, or direct HTML within the iframe element.
- Below is an example of an embedded map.

  ```html
  <h1>A Map from Openstreetmap.org Embedded with the iframe Element</h1>

  <iframe
    width="425"
    height="350"
    src="https://www.openstreetmap.org/export/embed.html?bbox=3.006134033203125%2C6.150112578753815%2C3.6357879638671875%2C6.749850810550778&amp;layer=mapnik"
    title="Map of Lagos area, Nigeria"
    style="border: 1px solid black"
  >
  </iframe>
  <br />
  <small>
    <a href="https://www.openstreetmap.org/#map=11/6.4501/3.3210">
      View Larger Map
    </a>
  </small>
  ```

**_Try interacting with the map by zooming in and out._**

**NOTE:** If you want to embed direct HTML within the iframe element you have to use the srcdoc attribute instead of src.

---

## 🧠 Key Takeaways

- Replaced elements are determined by external resources, not CSS
- Common replaced elements: `img`, `iframe`, `video`
- CSS can position replaced elements but not modify their content
- The `iframe` element embeds external content (videos, maps, web pages)
- Essential iframe attributes: `src`, `width`, `height`, `title`
- Use `allowfullscreen` for video embeds
- Always include a `title` attribute for accessibility
