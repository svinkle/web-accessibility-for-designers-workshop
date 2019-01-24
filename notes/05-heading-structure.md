# Heading structure

Setting in place a solid heading structure and design for any site or app is key for building an accessible experience.

It's important that not only the code making up the heading structure is linear and is in a logical order, but also visually as well. When someone who depends on **assistive technology** visits a new site or page that they've never been to before, they'll often first navigate by headings to get a sense of the content being offered on the page. It's the same idea, visually, for example someone reading through the headings of a newspaper; gather the general idea of the content available, then visit the sections of interest.

## Logical heading order is key

```html
<h1>Primary heading</h1>
<!-- … -->

<h2>Sub-section</h2>
<!-- … -->

<h3>Sub-sub-section</h3>
<!-- … -->

<h2>Sub-section</h2>
<!-- … -->
```

For example, in your HTML you'd start with a single `h1` heading as the primary title of the page, followed by an `h2` heading for each major sub-section of content. If there were any sub-sub-sections, those would feature `h3` headings. When a section of content is complete, the heading would return to the appropriate level to start the new section.

In addition to the HTML code behind the headings, the visual design of headings is also very important. Text sizes which go from large to medium to small denotes the content structure and related content. People with a **cognitive impairment** or **reading/learning disability** will greatly appreciate content being split into pieces with headings conveying the message that, "this is a new section of content." Without headings, large walls of content can be quite difficult for some people to consume and may even lead to a sense of overwhelm.

## Examples

- [No headings…](https://codepen.io/svinkle/full/ZRwYPm/)
- [Some headings-ish…](https://codepen.io/svinkle/full/QxYyyp/)
- [Solid headings](https://codepen.io/svinkle/full/PaVZzZ/)

Checkout these examples. Notice the increased readability and understanding of the text as the headings are added to the document.

_(Try out the last one using a screen reader)_

### ✅ [2.4.6 Headings and Labels](https://www.w3.org/TR/UNDERSTANDING-WCAG20/navigation-mechanisms-descriptive.html)

This comes back to 2.4.6 Headings and Labels which states

> "Headings and labels describe topic or purpose."
