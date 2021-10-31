# Title

**Watch the video [here](https://youtu.be/GRCs0_lzumA)**

## Prerequisites

- [Node.js](https://nodejs.org/en/download/)
- [Visual Studio Code](https://code.visualstudio.com/)

## Loose Agenda

- Create slideshows from markdown using Marp

## Step by Step

### Setup Playground

Create a directory for today's exercise and navigate to it in a terminal instance. 

Install marp by running `npm install -g @marp-team/marp-cli`

### Create our first slideshow

Create a new file named `sample.md`.

At the top of the file we can declare variables such as `theme` via the front matter syntax

```md
---
theme: uncover
---
```

Slide content is defined in standard markdown syntax and are separated by three dashes `---`. Let's define two slides per the following content.

```md
---
theme: uncover
---


# Marp Slide 1

Exciting content!

---

# Marp Slide 2

Slightly more exciting content!

```

Run `marp .\sample.md --pdf` from this directory to create a `sample.pdf` file.

### Themes

There are a variety of themes built into Marp. Let's swap the theme in `sample.md` to `gaia`.

```md
---
theme: gaia
---


# Marp Slide 1

Exciting content!

---

# Marp Slide 2

Slightly more exciting content!

```

Run `marp .\sample.md --pdf` from this directory to create a `sample.pdf` file.

### Additional Output types

Marp also supports output to PPTX or HTML.

Run `marp .\sample.md --pptx` from this directory to create a `sample.pptx` file.
Run `marp .\sample.md` from this directory to create a `sample.html` file.

Congratulations on a non-zero day!

## Additional Resources

- [Markdown Cheatsheet](https://www.markdownguide.org/cheat-sheet/)
- [Default Themes](https://github.com/marp-team/marp-core/tree/main/themes)
- [Marpit Documentation](https://marpit.marp.app/)
