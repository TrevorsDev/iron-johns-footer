## CSS Organization by Responsibility (Separation of Concerns)

### Summary:
This technique involves grouping CSS properties based on their purpose rather than by following the order of HTML or mixing everything together.

### Common Categories:
Layout → Handles positioning and spacing (e.g. display, flex, margin, grid, position, width, height)

Style/Visual → Controls look and feel (e.g. color, background, border, box-shadow)

Typography → Text styling (e.g. font-family, font-size, line-height, text-align)

Responsiveness → Media queries and breakpoints

Animations/Interactions → Transitions, transforms, hover/focus states

### Benefits:
Improves readability and maintainability

Easier to debug: Know where to look when something breaks

Scales better for large projects or teams

Encourages modular thinking

## Accessability Practice

Another thing that Ive learned through this process of building this custom website is the importance of accessability. In one example with this footer, I was creating forms. I wanted to test a modern asthetic by removing the outline on each input box where a user is going to write their text. I placed "outline: none" inside the correct selector but realized that people using screen readers or tabing through the form wont have any idea which element is currently active. I found that using the "::focused: pseudo class allows me more customization while maintaining a modern asthetic and answering to the missing accessability situation.


## Ideas on How to Handle Locations Page

I think that in both the nav and footer, simply clicking the locations page in order to send the user to a separate page that consists of all three locations with address and phone number below would be the best. Future development would allow clicking on each location in that page and in the nav dropdown menu and then having those links take you to each separate location website. ie Juniper, 18th, etc.

## Design Systems

Another new challenge from this footer project was learning to think in terms of design systems. Here I had to anticipate what code would be reused throughout the css file, and how I would section that code differently based on its given function. For example, creating a section in my CSS specifically for all the Layout structure, and setting a specific class to equal "width: 100%;" so that I could simply attach that class to other html components that would be styled in that way. Or      ".column {
    display: flex;
    flex-direction: column;
}"
creates a class that sets an element to have a column direction.
This complete reorganization of my CSS was a huge mindshift in how I thought of styling and structuring my files for organizatinal purposes, maintainability and the like.