# Build a Travel Agency Page

In this lab, you'll review working with HTML fundamentals by creating a web page for a travel agency. You'll work with images, the figure element, the figcaption element, the anchor element, and more.

Build an app that is functionally similar to this example project. Try not to copy the example project, give it your own personal style.

<video controls>
  <source src="./assets/videos/travel-agency-example-project.mp4" type="video/mp4">
</video>

---

## Objective:

- Fulfill the user stories below and get all the tests to pass to complete the lab.

## User Stories:

1. You should have a `DOCTYPE` declaration.
2. You should have an `html` element with `lang` set to `en`.
3. You should have a `head` element containing a `meta` void element with `charset` set to `utf-8`and a `title` with the text `Travel Agency Page`.
4. You should have a `meta` tag in your `head` element that contains a short description of your website for SEO.
5. You should have an `h1` element to present your travel destinations.
6. You should have a paragraph below the `h1` element introducing the travel opportunities.
7. You should have an `h2` element with the text `Packages`.
8. You should have a `p` element introducing briefly the various packages.
9. You should have an unordered list element with two list items. The two list items should have the text `Group Travels` and `Private Tours`, respectively. The text of each list item should be enclosed by an anchor element.
10. You should have an `h2` element with the text `Top Itineraries`.
11. You should have at least three `figure` elements, each containing an anchor element and a `figcaption` element.
12. The three anchor elements should have an `img` element with an appropriate `alt` attribute and a `src` attribute set to a valid image as their content. You can use `https://cdn.freecodecamp.org/curriculum/labs/colosseo.jpg`, `https://cdn.freecodecamp.org/curriculum/labs/alps.jpg`, and `https://cdn.freecodecamp.org/curriculum/labs/sea.jpg` if you would like.
13. All your five anchor elements should have an `href` attribute with the value of `https://www.freecodecamp.org/learn` and a `target` attribute with the value of `_blank`.

---

## Tests

1. Your travel agency page should have a `!DOCTYPE html` declaration.
2. You should have an `html` element with `lang` set to `en`.
3. You should have a `head` element within the `html` element.
4. You should have two `meta` elements within your `head` element.
5. One `meta` element should have a `name` attribute with value of `description` and a non-empty `content` attribute.
6. One `meta` element should have its `charset` attribute set to `UTF-8`.
7. You should have `title` element within your `head` element.
8. Your `title` element should have your travel agency name.
9. You should have a `body` element within your `html` element.
10. You should have an `h1` element to present your travel destinations.
11. You should only have one `h1` element.
12. You should have a `p` element below the `h1` element.
13. Your first `p` element should introduce the travel opportunities.
14. Your first `h2` element should have the text Packages.
15. You should have a `p` element below your first `h2` element.
16. Your second `p` element should introduce briefly the various packages.
17. You should have an unordered list element below your second `p` element.
18. You should have two items in your unordered list.
19. Both your list items should contain an anchor element.
20. The anchor element of your first list item should wrap the text `Group Travels`.
21. The anchor element of your second list item should wrap the text `Private Tours`.
22. You should have an `h2` element after your unordered list.
23. Your second `h2` element should have the text `Top Itineraries`.
24. You should have at least three `figure` elements.
25. Each `figure` element should contain an anchor element as its first child.
26. Each `figure` element should contain a `figcaption` element as its second child.
27. Each `figcaption` should contain some text.
28. Each of the `a` elements that are children of your `figure` elements should contain an image.
29. Each `img` element should have a valid `src` attribute.
30. Each `img` element should have an `alt` attribute with an appropriate value.
31. Each `a` element should have an `href` attribute with the value of `https://www.freecodecamp.org/learn`. Don't forget the links in the list items.
32. Each `a` element should have a `target` attribute with the value of `_blank`. Don't forget the links in the list items.
