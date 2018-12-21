# UI components with Sass

## Introduction
While working on UI design, few principles and guidelines are required to follow that help you design a standard and consistent experience throughout your products.
UI guidelines explain the anatomy of UI components and give understanding of their behavior by giving real examples.
These guidelines are usually defined at organization level and equally helpful for designers, developers and testers.

In this task you will have to implement several UI components from Audi's UI guideline.

Then you will need to create a page layout, making use of the created UI components.

> **Note**: All the components are already implemented and can be found on GitHub. While nothing restricts you from using the existing code, I am highly encouraging you to work on your own.

Let's start!

## Step 1
You will need to implement the following components:
- [Buttons](https://www.audi.com/ci/en/guides/user-interface/components/buttons.html)
    - Primary button
    - Secondary button
    - Text button
- [Typography](https://www.audi.com/ci/en/guides/user-interface/components/text.html)
    - Headings
    - Body copy
    - Caption
- [Card](https://www.audi.com/ci/en/guides/user-interface/components/card.html)

Have a look at them, think how you are going to implement them.
What questions do you have right away?
How will you name the components?
What variables are you going to use?

## Step 2
Create a working directory. Initialize `npm` in it.
```
npm init
```

Install the following packages (feel free to install more, this is just the required minimum):
```
gulp
node-sass
gulp-sass
gulp-sourcemaps
```

Configure your `gulpfile.js`. You may use [this](./gulpfile.js) as a starting point.

## Step 3
Now implement the UI components mentioned in the Step 1.
You don't need to implement the response effect for buttons.
You can use [Roboto](https://fonts.google.com/specimen/Roboto) instead of Audi's font.

Use this tips for code organization:
- Use CSS preprocessor.
- Use BEM.
- Put all variables into separate file.
- Create one file per component.
- Avoid unnecessary nesting.
- Prefer variables to specific values (i.e. `$color-accent` is better than `#e56567`).
- Use generic names for variables (i.e. `$color-accent` is better than `$color-coral`).

## Step 4
Using the UI components you've implemented in Step 3, create this layout:
- [Mobile (`<480px`)](./images/mobile-layout.png)
- [Tablet (`480px` - `1024px`)](./images/tablet-layout.png)
- [Desktop (`1024px+`)](./images/desktop-layout.png)

Make sure you use full width of the viewport at any device.

You can find the photo [here](./images/card-390x480.jpg).
Use CSS `grid` for positioning cards on the page correctly.

Put all the styles for this page into `layout.scss` file.
