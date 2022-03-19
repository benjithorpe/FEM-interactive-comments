# Frontend Mentor - Interactive comments section

This is a solution to the [Interactive comments section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/interactive-comments-section-iG1RugEG9).

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)
- [Acknowledgments](#acknowledgments)
- [How to contribute](#how-to-contribute)


## Overview

### The challenge

Users should be able to:

- View the optimal layout for the app depending on their device's screen size
- See hover states for all interactive elements on the page
- Create, Read, Update, and Delete comments and replies
- Upvote and downvote comments
- **Bonus**: If you're building a purely front-end project, use `localStorage` to save the current state in the browser that persists when the browser is refreshed.
- **Bonus**: Instead of using the `createdAt` strings from the `data.json` file, try using timestamps and dynamically track the time since the comment or reply was posted.

### Screenshot

![](./screenshot.jpg)

### Links

- Solution URL: [Solution URL here](https://github.com/benjithorpe/FEM-interactive-comments)
- Live Site URL: [Live site URL here](https://fem-interactive-comments.vercel.app/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
<!-- - CSS Grid -->
- Mobile-first workflow
- [Svelte](https://svelte.dev/) - JS framework


### What I learned

Install plugin to fetch data from a local file in the root of the project

```bash
npm add --save-dev @rollup/plugin-json
```
...then in the `rollup.config.js` you add this plugin:

```js
import json from '@rollup/plugin-json';

export default {
   // other stuff here
   plugins: [json()]
}
```
... in your svelte component you do

```js
import data from 'path/to/file.json';
```

### Continued development

- Event handlers

### Useful resources

- [Example resource 1](https://www.example.com) - This helped me for XYZ reason. I really liked this pattern and will use it going forward.
- [Example resource 2](https://www.example.com) - This is an amazing article which helped me finally understand XYZ. I'd recommend it to anyone still learning this concept.


## Author

<!-- - Website - [Add your name here](https://www.your-site.com) -->
- Frontend Mentor - [@benjithorpe](https://www.frontendmentor.io/profile/benjithorpe)
- Twitter - [@benjithorpe1](https://www.twitter.com/benjithorpe1)

## Acknowledgments

Thanks and appreciation to `@Rainlife` (in the svelte discord channel) for suggesting the
`@rollup/plugin-json` used to fetch data from a local file inside the root folder


## How to contribute

*Note that you will need to have [Node.js](https://nodejs.org) installed.*


## Get started

Clone the repo

```bash
git clone https://www.github.com/benjithorpe/FEM-interactive-comments
```

Install the dependencies...

```bash
cd FEM-interactive-comments
npm install
```

...then start [Rollup](https://rollupjs.org):

```bash
npm run dev
```

Navigate to [localhost:8080](http://localhost:8080). You should see your app running. Edit a component file in `src`, save it, and reload the page to see your changes.

By default, the server will only respond to requests from localhost. To allow connections from other computers, edit the `sirv` commands in package.json to include the option `--host 0.0.0.0`.