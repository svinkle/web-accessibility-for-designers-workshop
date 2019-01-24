# Animation

Have you ever had a bad day where you're just not feeling great? Perhaps you have a headache, or feeling nauseated from the night before? Then you go online to be greeted with a bunch of animation, scroll jacking, parallax motion, or a video background on a slide that it only make you feel worse! It happens to us all at some point or another.

Using animation on the web is a great way to bring a unique flare to your design and maybe add a bit of delight to your user experience. Well designed animations are informative; they let the user know something has taken place or are used to guide the user to a new task which needs attention. Ideally, animations would be useful, predictable, and consistent.

On the other hand, poor use of animations might be distracting, take the attention away from the current task, and might even leave someone feeling queasy and disoriented.

## What actually makes up a "poor" animation

Everyone will have a different reaction, or perhaps no reaction at all, to a piece of animation. For those who do experience a negative reaction, how to we avoid creating such an experience?

Here's a few points to consider when creating animations:

- **Size of movement.** Small or compact animations, like a loading spinner, are helpful. However, if there's something moving from one side of the screen to another, especially critical pieces of content, this can be problematic. Keep animations small and purposeful.
- **Direction and speed.** Parallax effects and scroll jacking, which tend to involve foreground and background elements moving at different speeds, or objects moving in different directions than expected, can cause issues. Allow the user to scroll at their own pace.
- **Distance.** For animations which seem to span large lengths of space, although only the size of a computer screen, can sometimes trigger a negative experience. Again, it's best to keep animations small and compact in order to avoid a negative user experience. Refrain from animating long lengths of content.

Animation is something that can unexpected, and when it's there, we typically don't have a whole lot of control over the experience. How can we ensure when animation is in use that we also create an accessible experience?

## Animation and accessibility

![A young woman holds her head in pain.](../slide-deck/images/vestibular-disorder.jpg)

How might adding animations to a website, app, or even an operating system, have a negative impact on those with a disability? Here's a couple ways:

- When it comes to someone with a **cognitive impairment**, setting in place a highly animated scene or activity upon completing an action, or having other moving pieces on the screen such as an auto-playing video or advertisement can be very distracting.
- For folks who are susceptible to motion sickness or **Vestibular issues**, some animation can very easily lead to feelings of nausea or vertigo.

## Animation example

Before we move on to discuss methods of ensuring a positive user experience with animation, let's _briefly_ look at a few examples…

- [Split Landing Page](https://codepen.io/2975/pen/WdMMaR)
- [Vimeo Cameo](https://vimeo.com/cameo)
- [Bolden](https://www.bolden.nl/)
- [Tank Design](https://tankdesign.com/)
- [The Boat](http://www.sbs.com.au/theboat/)

I think there's no doubt that there was a lot of effort and creativity put into making each of these sites. However, we might be able to conclude that inclusivity was not in mind when these user experiences were designed. Each example includes elements which would be problematic for some people with disabilities.

## How to ensure "accessible-friendly" animations

To be clear, the recommendation isn't to _not_ use animation as some animations can be quite helpful. Let's look at a few ways to create an accessible and inclusive experience through use of animation:

- **Design subtle animations.** Using animations in way that is subtle and used as a means to guide the user can be very helpful. Try to minimize animations which alter default speed, movement, and control that users are accustomed to.

  For example, when adding an item to a shopping cart, there could be an animation to highlight this activity as complete. Another example might be when submitting a dynamic form, animate an error or success message to draw the users attention to this area.

- **Animations should be easily understood and predictable.** In keeping with the "subtle" theme, animation should ideally be use in a way that people can understand the meaning behind the animation.

  An example of which; the classic loading spinner. This helps to inform the user that progress is being made and a background process is being run. It basically conveys the message, "Please be patient while we process your data."

- **Design a "no animation" state.** It is possible for people to "turn-off" animations at an operating system level. For example, the macOS Accessibility settings features the "Reduce motion" option.

  With this setting enabled, developers can take advantage of the CSS media query, "prefers-reduced-motion." Any styles applied within this media query would be those to produce the "no animation" state. This would be idea for any site featuring parallax scrolling; with this CSS media query in use, a developer could create a layout for a "static" alternative.

- **Allow animations to be paused.** If there are background videos, carousel sliders, or even animated GIF images on screen, provide a means for these types of content to be paused.

  Build the pause control into each element, but if there are many different animations to be halted, consider designing and implementing a global, "Pause all animations" control. Your users who are susceptible to motion sickness will thank you.

## ✅ [2.3.3 Animation from Interactions](https://www.w3.org/WAI/WCAG21/Understanding/animation-from-interactions.html)

This comes back to 2.3.3 Animation from Interactions which states

> "Motion animation triggered by interaction can be disabled, unless the animation is essential to the functionality or the information being conveyed."

## Exercise! 🎈

1.  Break into groups of 3 (or 4)
2.  Each group gets 1 balloon
3.  Designate someone to inflate and tie off the balloon
4.  Toss the balloon between your group members, and…
5.  Complete this task on your phone:
    - Find what's playing at a local movie theatre, this Saturday, 7pm
6.  Try not to drop the balloon!
