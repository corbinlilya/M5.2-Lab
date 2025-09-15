# web-dev-starter

This is a starter project for web development with no frameworks and minimal
dependencies. It is intended to be a starting point for web development projects
that are written in plain HTML, CSS, and JavaScript.

## Accessibility Lab Answers

### Color Contrast
Using the online tool in the reading, https://webaim.org/resources/contrastchecker/, using the background color hex #008000, and text color #2a2a2a.

These colors gave a ratio of 1.18:1, which failed every contrast test. To fix this, we can change the background to white and keep the text color.

### Semantic HTML

The navigation, query, related, and audio elements are all accessible with keyboard. The only interactive element that is not
accessible by keyboard is the show comments button, as pressing return on the button does not toggle the show comments. But,
it only navigates through buttons and doesn't go through the headers or different parts of the article, it only goes to
interactive elements.

To make the article text more accessible, we can use clear structure and headings.

For navigation elements, we can wrap those in the `<nav>` element.

### Images
To fix the images to make them more accessible, we can add
alt tags to each image.

### Audio Player
For hearing impaired people, we can add a transcript as an alternative below the audio player. If it was a long audio clips, I
wouldn't manually transcribe, but it was short so I added a show/hide transcript button.

### Input Forms

We can add the aria-label to add a label that is not visibile to sighted users. For the comment input, we can add `<label>` elements with "for" attributes to associate them to the input, matching the input id.

### Tables
For the table of information, we can make it more accessible by adding scopes to each column, and start of each row, and changing each column and start of each row to `<th>` elements. We can add an aria-describedby label and `<caption>` to create a readable summary for the table and describe the table.

### Other Changes
We can add tabindex to elements that we want to be tabbable that we want to be keyboard accessible. If I was navigating an article with my keyboard, and it was a long scrollable page, tabbing through headers might be useful. Also, the header is currently just a div, so we can change that to a `<header>` tag. As well, we can change the `<div class="secondary">` to an aside, which is what it visibily is, and keep the class for CSS. We can also add a lang attribute to the `<html>` tag.


## Getting Started

To get started, clone this repository and run the following commands:

```bash
npm install
```
This will install the necessary dependencies for the project.

## Development

It is recommended to use the VSCode Live Server extension to run the project
locally. This will allow you to see changes in real-time as you make them. There
is no need to run a build process or refresh the page manually. Additionally,
you do not need to setup a local server to run the project.

## Testing

To run the tests for the project, run the following command:

```bash
npm test
```
