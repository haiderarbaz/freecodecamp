# 🏷️ Working with Images and SVGs

[⬅️ Back to BASICHTML.md](../BASICHTML.md)

In this section, you will learn how to work with SVGs and learn about techniques for optimizing your images.

1. [What Are Common Ways to Optimize Media Assets?](https://www.freecodecamp.org/learn/full-stack-developer/lecture-working-with-images-and-svgs/what-are-common-ways-to-optimize-media-assets)

2. [What Are the Different Types of Image Licenses, and How Do They Work?](https://www.freecodecamp.org/learn/full-stack-developer/lecture-working-with-images-and-svgs/what-are-the-different-types-of-image-licenses)

3. [What Are SVGs, and When Should You Use Them?](https://www.freecodecamp.org/learn/full-stack-developer/lecture-working-with-images-and-svgs/what-are-svgs)

---

## Short Summary from the above docs

This summary helps you quickly revise the key takeaways from the freeCodeCamp “Working with Images and SVGs" docs.

---

## 📋 Table of Contents

- [▶️ Common Ways to Optimize Media Assets](#▶️-common-ways-to-optimize-media-assets)
- [🖼️ Types of Image Licenses](#🖼️-types-of-image-licenses)
- [🎨 SVGs](#🎨-svgs)
- [🧠 Key Takeaways](#🧠-key-takeaways)

---

## ▶️ Common Ways to Optimize Media Assets

- There are three factors to consider when using media, such as images, on your web pages:

  1. The size,

  2. The format, and

  3. The compression.

- When you are building a website, you'll often style images to display in a specific size.

- For example,

  - You might have an image display at a 640x480 resolution.

  - 640 represents the width while 480 represents the height in pixels.

- When preparing your image you want to scale it to a 640x480 size to match that styling.

- If you serve an image that is 1920x1080 but you are styling it to be much smaller, you're requiring your users to download unnecessary data.

- A smaller resolution results in a smaller file size.

- The next thing to consider is your file format.

- Two of the most common file formats are

  1. PNG and

  2. JPG,

- But these are no longer the most ideal formats for serving images.

- Unless you need support for older browsers, you should consider using a more optimized format, like WEBP or AVIF.

- Finally, you can run compression algorithms on your images.

  - A compression algorithm is used to reduce the size for files or data.

- There are options like pngcrush to compress your images locally, or you can use online compression tools.

- However, it's worth noting that specific file formats, such as JPG, are not lossless.

  - Lossless means that the original data can be perfectly reconstructed from the compressed data.

- If you try to compress a JPG image, it will result in a degraded quality.

**You should keep all these things in mind when selecting images for your web pages.**

---

## 🖼️ Types of Image Licenses

- Images are considered intellectual property, this means that they are protected by copyright regulations, most often belonging to the creator.

- By default, images are released as `all rights reserved`.

  - The creator, or publisher sometimes, holds all copyright for the image.

- This means that you cannot use them in your web page unless you do one of three things:

  1. Obtain written permission from the copyright holder,

  2. Purchase a license from the copyright holder, or

  3. Incorporate the image in a way that falls under fair use.

- That third point is a bit tricky.

  - Fair use requires that your use of the image is both limited and transformative.

  - Some examples of fair use would be to comment on or review the art or create a parody of the image.

- Some images might be released under a permissive license, like a Creative Commons license, or the BSD license that freeCodeCamp uses.

- These images are available for use in your website, but you'll need to read the license to understand the rules you need to follow when using these images.

- For example,

  1. You might be required to make your website open source, or

  2. You may not be permitted to modify the image in any way.

- Finally, some images may be released to the public domain.

- An image under the public domain has no copyright attached to it and is free to be used without any restrictions.

- Images licensed specifically under the `Creative Commons 0` license are considered public domain.

- Most search engines will allow you to filter image results by a license.

- There are also sites like `Pixabay` and `Unsplash`, which offer free-to-use images.

**Always be mindful of the copyright and licensing when you use an image in your website.**

---

## 🎨 SVGs

**First, you need to understand how images work**.

- Common image formats like PNG and JPG are classified as raster formats.

  - This essentially(raster) means that they are pixel-based, with the data tracking the color value in each pixel.

- A large downside of raster based images is that they do not upscale well.

- If you've ever tried to make a PNG larger, you may have seen that it becomes pixelated, or blurry.

**There comes SVG**

- An SVG is a different kind of image.

  - SVG stands for a scalable vector graphic.

- A vector graphic tracks data based on paths and equations to plot points, lines, and curves.

  - What this really means is that a vector graphic, like an SVG, can be scaled to any size without impacting the quality.

- SVGs specifically have the added benefit of storing data in XML.

  - This means you can use them directly in your code as raw HTML with the `svg` element.

  - It also means you can programmatically change the color of the image.

- For Example,

  - To change the smiley face to red, change the `fill="yellow"` to `fill="red"`.

  ```html
  <svg
    width="100"
    height="100"
    viewBox="0 0 100 100"
    xmlns="http://www.w3.org/2000/svg"
  >
    <circle
      cx="50"
      cy="50"
      r="45"
      stroke="black"
      stroke-width="4"
      fill="yellow"
    />
    <circle cx="35" cy="40" r="5" fill="black" />
    <circle cx="65" cy="40" r="5" fill="black" />
    <path
      d="M35 65 Q50 80 65 65"
      stroke="black"
      stroke-width="4"
      fill="transparent"
    />
  </svg>
  ```

  - The basic elements for the example:

  - The `svg` element is the container for the whole drawing. It sets up the space where all the shapes appear. Everything you want to draw with SVG, such as circles, lines, or paths, goes inside the `svg` element.

  - The `circle` element is used to make the face and the eyes. One large circle forms the yellow face, and two smaller circles make the eyes.

  - The `path` element is used to draw the smile. It creates a curved line for the mouth.

  - Each SVG element has attributes that control its appearance and position within the drawing area.

- Below are few more examples.

  - To change the color for any of the examples, update the value for the `fill` attribute to any named color like `red`, `green`, `blue`, `yellow`, etc

  ```html
  <!-- Star Icon -->
  <svg
    width="50"
    height="50"
    viewBox="0 0 24 24"
    fill="gold"
    xmlns="http://www.w3.org/2000/svg"
  >
    <path
      d="M12 2L14.9 8.6L22 9.3L17 14.1L18.3 21.2L12 17.8L5.7 21.2L7 14.1L2 9.3L9.1 8.6L12 2Z"
    />
  </svg>
  ```

  ```html
  <!-- Heart Icon -->
  <svg
    width="50"
    height="50"
    viewBox="0 0 24 24"
    fill="crimson"
    xmlns="http://www.w3.org/2000/svg"
  >
    <path
      d="M12 21.35L10.55 20.03C5.4 15.36 2 12.28 2 8.5C2 6 4 4 6.5 4C8 4 9.5 4.8 10.5 6.09C11.5 4.8 13 4 14.5 4C17 4 19 6 19 8.5C19 12.28 15.6 15.36 10.45 20.04L12 21.35Z"
    />
  </svg>
  ```

  ```html
  <!-- Checkmark Icon -->
  <svg
    width="50"
    height="50"
    viewBox="0 0 24 24"
    fill="green"
    xmlns="http://www.w3.org/2000/svg"
  >
    <path
      d="M20.29 5.71L9 17L3.71 11.71L5.12 10.29L9 14.17L18.88 4.29L20.29 5.71Z"
    />
  </svg>
  ```

- **_Open these code in your fav IDE or text editor and play with the code._**

### When to use an SVG?

- A great use case is for icons.

  - If you want to create custom bullet points, or add icons to your links to represent social media platforms, using SVGs is the best approach.

- One of the most popular icon libraries, Font Awesome, uses SVG images for their icons.

- SVGs are also great for webpage logos, because they scale perfectly.

- They allow you to adapt your layout to any responsive design you need.

**Next time when you have an SVG locally, try opening it with a text editor and playing with the code.**

## 🧠 Key Takeaways

- Optimize images by adjusting size, format, and compression
- Use modern formats like WEBP or AVIF for better performance
- All images are copyrighted by default—respect licensing requirements
- Fair use, Creative Commons, and public domain images have different usage rules
- SVGs are vector-based and scale infinitely without quality loss
- Raster images (PNG, JPG) are pixel-based and become blurry when enlarged
- Use SVGs for icons and logos; use raster formats for photos
- SVG code can be edited directly in HTML and styled with CSS
