# typewriter-effect-in-pure-css
This works well for hero sections where you want to cycle through a handful of words or roles without relying on JavaScript. Developers typically use them for their portfolio sites.  Just make sure the background behind the text is a solid color that matches the page, otherwise, the typing effect can expose the edge of the animation.

Source: https://prismic.io/blog/css-animation-examples

This works well for hero sections where you want to cycle through a handful of words or roles without relying on JavaScript. Developers typically use them for their portfolio sites.

Just make sure the background behind the text is a solid color that matches the page, otherwise, the typing effect can expose the edge of the animation.

Prismic integration
This animation is one of the few in this guide that isn't editor-friendly. Since every keyframe is based on the exact number of characters in each word, the CSS can't simply pull values from a Key Text or Rich Text field.

One way around that is to store the words in a repeatable Group field and generate the keyframes when the Slice renders. A helper like buildTypewriterKeyframes below can calculate the timing for each word automatically, so editors can add, remove, or reorder words without having to ask developers to manually update the animation.
