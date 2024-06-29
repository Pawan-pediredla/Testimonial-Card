Project brief :

In this challenge, you will develop a card featuring a user testimonial, including a profile image, name, username, and the testimonial body.


Implementation requirements :


Design fidelity: Aim to follow the design as closely as possible. All elements in the design should be present, using the specified text color, font size, font weight, spacing, dimensions, etc.

Cross-browser compatibility: Check that your solution works for major browsers including Chrome, Firefox and Safari.

[Stretch goal] Handle long strings: In reality, the person's name and testimonial can be extremely long. The UI should be able to accommodate extremely long strings by either wrapping to the next line, truncating, or both
.
[Stretch goal] Performance optimization: Optimize image assets and code for quick load times, ensuring a smooth and responsive user experience.

[Stretch goal] Accessibility and semantics: Follow best practices for web accessibility, such as using semantic HTML and ARIA roles where necessary and using proper alt tags for images.


Relevant concepts
These CSS concepts will be useful for this challenge.

Box model: Understanding padding, borders, and margins is necessary for achieving the desired layout.
Flex: Flex layouts are useful for displaying the image and text side-by-side. While flex is not the only way to achieve the layout, it is the modern way of doing so.
Recommended approach
Build the page layout: Render a background color for the page. Within the page, add a horizontally-centered card that is a fixed distance of 200px from the top of the page.
Build the card and its contents: Display the avatar image, name, username, and testimonial message.
Card structure
Build the card container first, then add the contents starting from the top.
Use semantic HTML elements to create containers for different parts of the card. For instance, you might have one <div> for the card itself, another <div> wrapping the user avatar and name, and a <p> for the testimonial message.
Use an <img> tag to display the avatar picture, making sure to provide alt attributes for accessibility.
Card layout
Observe that the card has a fixed width of 340px and is a fixed distance of 200px from the top of the screen (it is not vertically centered!).

Set a fixed width and margin-top for the card.
The card should not have a hardcoded height value; its height should be according to the vertical space taken up by its contents. This is the behavior by default in CSS, so there are no extra steps needed.
To horizontally center the card on the page, a simple way would be margin-left: auto; margin-right: auto or to make the card parent display: flex; justify-content: center.
Use modern display properties like flex and grid. display: flex can be used to make the image and the words side-by-side.
Styling the card and its contents
When styling, use classes to apply styles to specific elements as opposed to inline styles. There can be more than one testimonial card per page, using classes will allow you to apply the styles to another testimonial card instance.
Notice that the card has a box shadow, a background color and rounded corners! Be sure to add the necessary styling.
Refer to the style guide for the appropriate typography values and colors to use.
Round images can be achieved using the border-radius property – use a value of at least half the height of the image, or some really huge value like border-radius: 9999px.
