# Focus indicator

One of the most basic aids to help people navigate an app with ease and confidence (and is baked in to every site by default) is the focus indicator.

What is the focus indicator? It's the visual indicator of where you currently are on a page when navigating by keyboard alone.

Load up your favorite site and start pressing the `Tab` key. Is there any indication of where the cursor currently is on the page? If you're in Chrome or Safari the default indicator is a blue outline, where Firefox and Internet Explorer/Edge features a dashed black outline.

> If you can't see where the cursor currently resides on the page, you've got an accessibility issue

For people with **motor disabilities** or any other impairment (temporary or permanent) which prevents use of the mouse, navigating with the keyboard is the next best option.

What happens when you use the `Tab` key on a site is the keyboard cursor will move from one HTML element to the next. The elements highlighted are naturally focusable. Elements such as links, `button`s, form `input`s, etc all receive keyboard focus by default and should highlight when the cursor moves from one to the next.

Sometimes, the request is made to remove the focus indicator outline. This is usually a result of the outline being displayed on mouse interaction which can be viewed as a negative cosmetic result. While it is **strongly** recommended to _not_ remove the default indicator, there are a few work-arounds which could be used as a replacement.

## Custom focus indicator

Using CSS it is possible to create your own focus indicator. With a bit of code such as…

```css
*:focus {
  outline: solid 3px red;
}
```

…you can create a custom focus indicator. This places a solid red outline around focusable elements.

When implementing a custom outline, there are a couple things to keep in mind:

- Ensure the contrast ratio of the indicator against the background is high. If people can't see the focus indicator the its purpose is lost.
- Make it consistent. Since a custom focus indicator will be unexpected on first visit, it's a good idea to keep things consistent and predictable throughout the user experience of the site.

## Detect keyboard/mouse usage

There's been lots of great work done recently on detecting when someone's using a mouse or a keyboard to navigate site content. In doing so, designers are able to create a custom, highly visible focus indicator for keyboard users only. Mouse users would be free to rely on only the mouse cursor as their indicator.

This technique is not yet built directly into browsers. However, there are third-party code snippets (also called a "polyfill") available to gain this functionality.

Two of which worth checkout out include:

- [focus-visible](https://github.com/WICG/focus-visible)
- [what-input](https://github.com/ten1seven/what-input)

## ✅ [2.4.7 Focus Visible](https://www.w3.org/TR/UNDERSTANDING-WCAG20/navigation-mechanisms-focus-visible.html)

This comes back to WCAG 2.4.7 Focus Visible which states

> "Any keyboard operable user interface has a mode of operation where the keyboard focus indicator is visible."

## Exercise! ⌨️

Go to your browser and open up some of your favorite sites. Try navigating with just the `Tab` key. Are you able to see where the keyboard cursor is currently placed? Or is there any focus indicator at all?
