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
