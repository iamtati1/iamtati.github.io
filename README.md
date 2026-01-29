# iamtati.github.io
Questions:

**1. Share one technical concept that you developed greater mastery over in this project. Demonstrate how you understand that concept by sharing your mental model of the concept. Then, show how you used that concept in your project.**

One technical concept I really developed mastery over in this project is CSS styling and layout, especially ***Flexbox***. I think of elements on a page as flexible boxes that I can stretch, center, or space however I need using properties like display: `flex;`, `justify-content`, and `align-items`. My mental model is that each container is like a mini layout puzzle: I can control how the pieces inside it behave and interact, which gives me full control over spacing, alignment, and responsiveness.

I used this concept throughout my portfolio. For example, I applied `Flexbox` to my projects grid to make the project cards line up neatly and adjust on smaller screens. I also used it in my navigation bar and home buttons to keep everything aligned. 

Beyond layout, I applied what I learned about `CSS` styling colors, `hover` effects, `border-radius`, shadows to make each section visually cohesive. When I needed guidance or inspiration, I asked AI to suggest color palettes and design ideas, which helped me create a polished portfolio that’s both functional and visually appealing.




**2. Choose one project requirement that you found challenging and are proud of implementing. Describe what made it challenging and how you were able to implement the requirement by walking through your code as succinctly as possible. Remember that your audience does not know your code nearly as well as you do so you’ll have to break it down in a logical manner for them to quickly understand it.**



One project requirement I found challenging was creating the `project-card` layout and aligning the cards in a grid. I knew how to style cards and how to make grids separately, but combining both—so each card contained an image, description, and links while staying neatly aligned—was tricky.

To implement this, I first styled the individual cards:

```
.project-card {
    background-color: var(--bg-card);
    border-radius: var(--radius-lg);
    padding: 2rem;
    box-shadow: var(--shadow-soft);
    transition: transform 0.35s ease, box-shadow 0.35s ease;
}

.project-card:hover {
    transform: translateY(-4px);
    box-shadow: var(--shadow-hover);
}
```

This gave each card a clean background, soft corners, padding for spacing, and a subtle shadow to make them pop. I also added a `hover` effect for interactivity.

Next, I used a grid container to align all the project cards:
```

.projects-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
    gap: 24px;
    margin-top: 40px;
}

```

Here, display: grid created a flexible layout. The repeat`(auto-fit, minmax(280px, 1fr))` allowed cards to automatically adjust their size based on the screen width, keeping them responsive. The `gap` created consistent spacing between cards, and `margin-top` added some space from the section heading.

Finally, I styled the card content inside each card, including the `image`, `title`, `description`, and `links`. I used `padding` inside the content container and set spacing between text and links to ensure everything looked neat and readable.

By breaking the problem into grid layout, card styling, and content spacing, I was able to combine all these concepts to make the cards visually appealing, interactive, and fully responsive.





**3. How did you leverage AI to assist your development of this project?**

I leveraged AI to build on what I already knew. While I was comfortable implementing key CSS and Flexbox concepts individually, I found it challenging to combine them effectively—sometimes styles would override each other or not behave as expected. AI helped me break down these challenges, see how the different pieces could fit together, and troubleshoot issues more efficiently, allowing me to move forward confidently. Overall Ai was a big help!

**AI Usage Document Link**

[link-to-AI-Usage-Document](https://docs.google.com/document/d/1nMSvCBU2pngqc2uU65C6mlp-sNYiSfdJuZJkz_4skYE/edit?usp=sharing)

(Command + Click)

**Deployment**

This portfolio is deployed using GitHub Pages and is accessible at https://iamtati1.github.io. 

I tested the deployed site across desktop, tablet, and mobile breakpoints to ensure layout consistency and functional navigation.

/*comment*/