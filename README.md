

![Github Forks](https://img.shields.io/github/forks/senli1073/senli1073.github.io?style=flat)
![Github Stars](https://img.shields.io/github/stars/senli1073/senli1073.github.io?style=flat)
![License](https://img.shields.io/github/license/senli1073/senli1073.github.io)
![Last Commit](https://img.shields.io/github/last-commit/senli1073/senli1073.github.io)

# A simple Github Pages template for academic personal website with a leadership section

## Preview
[![Screenshot of the Website](https://raw.githubusercontent.com/shotgunosine/shotgunosine.github.io/main/screenshot_full.png)](https://dylannielson.com/)


## Introduction

This is an academic personal website template based on [bootstrap](https://github.com/StartBootstrap/startbootstrap-new-age).

The template is designed to integrate Markdown files as content input.  There's no need to compile the webpage before deployment.  Upon loading, the Markdown files are automatically parsed and embedded into the page.

This template supports LaTeX formula input. You can use `$...$` and `\(...\)` as delimiters for inline-math, or use `$$...$$` and `\[...\]` as delimiters for display-math. Macros such as `\ref{...}`, `\eqref{...}`, and `\begin{equation}...\end{equation}` are also supported. See [MathJax](https://docs.mathjax.org/en/latest/index.html) for more details.

:milky_way: Demo: https://dylannielson.com


## Getting Start
### 1. Fork this repository
The repository name should be `<username>.github.io`, which will also be your website's URL.

### 2. Download the repo
Go to the folder where you want to store your project, and clone the new repository:
```
git clone https://github.com/<username>/<username>.github.io.git
```

### 3. Delete my content
(This bit's untested, let me know if it doesn't work)  
(1) Go to the folder where you cloned the repo
```
cd <username>.github.io
```
(2) Reset the main branch so it exactly matches the template branch
```
git reset --hard template
```

(3) Push your changes back to github
```
git push origin main --force
```
Now you can edit your main branch to add your content.

### 3. Edit page content

(1) If you're not already there, go to the folder cloned the repo.  
The directory structure is as follows:  

```.
.
├── contents
└── static
    ├── assets
    │   └── img
    ├── css
    └── js
```

(2) Modify the content of each section, which corresponds to `contents/*.md`. If you search for TOKUM you should find all the things that need to be changed. Refer to [markdown guides](https://www.markdownguide.org/) for formatting. You can see an example of how to embed an image [here](https://github.com/Shotgunosine/shotgunosine.github.io/blob/bdf2170d70a49d5066e6566863c457ea1acb7216/contents/leadership.md?plain=1#L1)

(3) If you want to have different sections, you'll need to edit [this part of index.html](https://github.com/Shotgunosine/shotgunosine.github.io/blob/fb0b8c020c223f686c2312ab1bcfecd7b3d73c8a/index.html#L97-L113), [this line of the script](https://github.com/Shotgunosine/shotgunosine.github.io/blob/fb0b8c020c223f686c2312ab1bcfecd7b3d73c8a/static/js/scripts.js#L5), and add the appropriatly named markdown file to the contents directory.

(3) Adjust the title, copyright information, and other text of the website in `contents/config.yml`

(4) Replace background image and photo with new ones for your web pages in `static/assets/img/`

(5) Replace your photo in `static/assets/img/`

(6) Use [a favicon generator](https://favicon.io/favicon-converter/) to convert your photo into an icon for the browser tab and replace all of the files under assets.

(7) Push it: 
```
git commit -am 'init'
git push
```

### 4. Enjoy

Fire up a browser and go to `https://<username>.github.io`



## License

Original Template: Copyright Sen Li, 2023. Modified by Dylan Nielson, 2025. Licensed under an MIT license. You can copy and mess with this template.  
Content: Copyright Dylan Nielson, 2025, free to use on [CC-By-NC 4.0](https://github.com/idleberg/Creative-Commons-Markdown/blob/main/4.0/by-nc-nd.markdown)

