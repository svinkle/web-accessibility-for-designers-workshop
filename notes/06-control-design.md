# Control design

What is actually meant by, "control design?" This is referring to the look and feel of the focusable elements: links and `button`s.

In modern web design, it's not uncommon to see links which look like `button`s; text with a background color and rounded borders, or a solid outline and transparent background. It's slightly less common to see `button`s which look like links, but it does happen.

## Control design and accessibility

![An underlined link with the text, 'Link'. A button with the text, 'Button'.](../slide-deck/images/link-button.png)

When it comes to accessibility best practices, the ideal design for each control would be something of a traditional look; colored text with an underline to denote a link and a solid background color with slightly rounded corners to denote a `button`.

Why is it so critical to usability and accessibility for these elements to appear in this manner? Here's a few reasons:

- Having controls designed in a consistent manner allows people with a **cognitive impairment** to identify and use the control with confidence, that it will result in meeting their expectations.
- When someone with a **motor disability** relies on voice dictation software and they announce, "click Submit button" when really the `button` is actually a link element, their command will not work.
- When links are only distinguished by color alone, folks with **color blindness** or **low-vision** may not be able to perceive the link for a link and miss it completely.

With links designed like links and `button`s designed like `button`s, everyone will benefit from the clear indication of which is which and will be able to use the controls with confidence. The idea is to avoid activating something that they weren't expecting, causing them more work to undo the previous action.

In other words, make sure things are clear, consistent, and obvious.

## Hover, focus, and active state

Another consideration when designing interface controls; the hover, focus, and active state.

### Hover state

![An animated GIF highlighting mouse hover styles; from red to dark red.](../slide-deck/images/hover.gif)

```css
a:hover {
  color: FireBrick;
}
```

The hover state comes into play when someone using a mouse hovers over an interactive element. Changing the visual aspect to something like a background color or an underline greatly helps to generate a visual cue that the element they're currently hovering on is interactive. It provides a sense of reassurance that this thing they're currently hovering over is indeed clickable.

### Focus state

![An animated GIF highlighting keyboard focus styles.](../slide-deck/images/focus.gif)

```css
a:hover, a:focus  {
  color: FireBrick;
}
```

Likewise, when someone is using a keyboard to navigate through a page, the focus state should be made available to alter the visual aspect in order to denote the current position of the keyboard cursor on the page.

It's generally best practice to include focus visuals along side hover styling in order to provide a consistent visual treatment.

### Active state

![An animated GIF highlighting mouse activation styles; dark red to black.](../slide-deck/images/active.gif)

```css
a:active {
  color: Black;
}
```

In addition to the hover and focus state, the active state is also available.

The active state shows only when an element is currently being interacted with. For example, when someone clicks down on a link and then releases the mouse button, that in-between state is the active state.

Including a unique active state style helps people with **motor impairments** or even **dyslexia** as when an item is interacted with, the active state serves as a confirmation and reassurance that the element was clicked.

I know I'm showing some code here but what's important is to include each state in your design and clearly annotate which color variation represents which state. This way a developer can implement these when they start their work.

## ✅ [2.4.4 Link Purpose](https://www.w3.org/WAI/WCAG21/Understanding/link-purpose-in-context.html)

This comes back to 2.4.4 Link Purpose which states

> "The purpose of each link can be determined from the link text alone or from the link text together with its programmatically determined link context."
