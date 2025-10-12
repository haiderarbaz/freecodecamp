# 🏷️ Understanding how HTML Affects SEO

[⬅️ Back to BASICHTML.md](../BASICHTML.md)

This section covers how HTML code impacts search engine optimization.

1. [What Is the Role of the Meta Description, and How Does It Affect SEO?](https://www.freecodecamp.org/learn/full-stack-developer/lecture-understanding-how-html-affects-seo/what-is-the-role-of-the-meta-description)

2. [What Is the Role of Open Graph Tags, and How Do They Affect SEO?](https://www.freecodecamp.org/learn/full-stack-developer/lecture-understanding-how-html-affects-seo/what-is-the-role-of-open-graph-tags)

---

## Short Summary from the above docs

This summary helps you quickly revise the key takeaways from the freeCodeCamp “How HTML affects SEO” docs.

---

## 📋 Table of Contents

- [🔍 Meta Descriptions and SEO](#🔍-meta-descriptions-and-seo)
- [📱 Open Graph Tags](#📱-open-graph-tags)
- [🧠 Key Takeaways](#🧠-key-takeaways)

---

## 🔍 Meta Descriptions and SEO

**What Is the Role of the Meta Description, and How Does It Affect SEO?**

- SEO, or Search Engine Optimization, is a practice that optimizes web pages so they become more visible and rank higher on search engines.

- One way to improve your site's SEO, is to provide a short description for the web page using the `meta` element.

- Below is an example of using the meta element to set a page description for a gardening site:

  ```html
  <meta
    name="description"
    content="Discover expert tips and techniques for gardening in small spaces, choosing the right plants, and maintaining a thriving garden."
  />
  ```

  - By setting the `name` attribute to `description`, it ensures that browsers, search engines, and other web tools correctly interpret this metadata.

  - The `content` attribute is where you will place your description.

  - It is recommended that you keep your descriptions short and concise. This is because search engines will often truncate the description based on the results page layout.

- Similar to other types of meta elements, the meta description will not be visible on the web page itself.

- One place where the page description can be found is in the search engine results page snippet.

- Below are some examples of page result snippets for freeCodeCamp's subreddit and GitHub repositories:

  ```markdown
  **Example search result snippets:**

  > \FreeCodeCamp: This is the official subreddit for the freeCodeCamp.org community. Learn to code for free together with millions of other people...

  > Our full-stack web development and machine learning curriculum is completely free and self- paced. We have thousands of interactive coding challenges to help you...
  ```

  - In the examples, each of the page descriptions are located just beneath the site links.
  - Within a couple of seconds, users can get a general sense of what the page is about and decide to click on the links for more information.

- Even though meta descriptions won't directly affect a site's ranking on search engine, having a strong description could result in more traffic to your website.

---

## 📱 Open Graph Tags

**What Is the Role of Open Graph Tags, and How Do They Affect SEO?**

- The open graph protocol enables you to control how your website's content appears across various social media platforms, such as Facebook, LinkedIn, and many more.

- By setting these open graph properties, you can entice users to want to click and engage with your content.

- You can set these properties through a collection of `meta` elements inside your HTML `head` section.

- The first important OG property to include would be the `title`.
- Below is an example of setting the OG `title` for the freeCodeCamp homepage:

  ```html
  <meta content="freeCodeCamp.org" property="og:title" />
  ```

  - For the `property` attribute, you will need to specify that it is `og:title`.
  - The `content` attribute is where you will write the title you want displayed for social media sites.

- The second important OG property would be the `type`.
- Below is an example of using the OG `type` for the freeCodeCamp homepage:

  ```html
  <meta property="og:type" content="website" />
  ```

  - The `type` property is used to represent the type of content being shared on social media. Examples of this content include articles, websites, videos, or music.

- The third important OG property would be the `image`.
- Below is an example of setting the OG image for the freeCodeCamp homepage:

  ```html
  <meta
    content="https://cdn.freecodecamp.org/platform/universal/fcc_meta_1920X1080-indigo.png"
    property="og:image"
  />
  ```

  - In this example, the open graph image is pointing to the freeCodeCamp logo.
  - All of these images should be high quality with good dimensions and ratios.
  - Most social media platforms will include criteria for image requirements to help you ensure that your content displays well on their site.

  - For example, the developers.facebook.com documentation page states:

    **_"use images that are at least 1200 by 630 pixels for the best display on high resolution devices. At the minimum, you should use images that are 600 by 315 pixels to display link page posts with larger images."_**

- The fourth important OG property would be the `url`.
- Below is an example of setting the OG url for the freeCodeCamp homepage:

```html
<meta property="og:url" content="https://www.freecodecamp.org" />
```

**Note:**

- There are many more OG properties that you can set, like `description`, `audio`, `video` and `locale`.
- However, the open graph `url`, `image`, `type`, and `title` are the most important ones to include.

**How do these open graph properties affect Search Engine Optimization?**

_When your content is shared on social media, well-crafted OG properties can enhance the appearance for your content in users' feeds. This can lead to higher click-through rates which could signal to search engines that your content is relevant and engaging._

---

## 🧠 Key Takeaways

- Meta descriptions improve click-through rates from search results
- Open Graph tags control how content appears on social media
- Essential OG properties: title, type, image, and URL
- High-quality images (minimum 1200×630px) are recommended
- Well-optimized HTML can indirectly boost SEO through user engagement
