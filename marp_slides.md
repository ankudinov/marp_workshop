---
marp: true
author: Petr Ankudinov
theme: default
class: invert
backgroundImage: "linear-gradient(to bottom, #1e3744, #301B29)"
# backgroundImage: "linear-gradient(to right, #0f2027, #203a43, #2c5364)"
# backgroundImage: "linear-gradient(to bottom, #004643, #001e1d)"

---
# How to Build Marp Slides

Hello World!

![bg](img/pexels-renato-rocca-9279669.jpg)

---

# Use Cases For Marp

- Repeatable way to build slide
- Integrate slide with some repository
- Sharing

Marp is not the only framework to build slides!

---

# How to Change Theme

Nice and dark. 🌔 <- with emoji

```markdown
---
marp: true
author: Petr Ankudinov
theme: default
class: invert
```

---

# To Get Free Pictures

![bg right](img/pexels-adrien-olichon-2823459.jpg)

Use:

- [Pexels](https://www.pexels.com/)
- [Unsplash](https://unsplash.com/)

How to work with images:

- [image syntax](https://marpit.marp.app/image-syntax)

If you can - add a reference to the author or collection.

---

![bg blur:2px](img/pexels-adrien-olichon-2823459.jpg)
![bg opacity:.7](img/pexels-adrien-olichon-2823459.jpg)
![bg sepia](img/pexels-adrien-olichon-2823459.jpg)

---

# More Marp Themes

Marp community themes:

- [Dracula](https://draculatheme.com/marp)
- [Beam](https://rnd195.github.io/marp-community-themes/theme/beam.html)
- [Marpstyle](https://github.com/cunhapaulo/marpstyle)

---

# Using Community Themes

- Add CSS from some community repos
- add following VSCode settings:

```json
{
    "markdown.marp.themes": [
        "./themes/dracula.css",
        "./themes/beam.css",
        "./themes/jobs.css",
        "./themes/einstein.css",
    ]
}
```

- Use theme: `theme: <theme-name>`
- Update the workflow: `--theme ./themes/dracula.css ... etc.`

---

# Using Gradient Background

```yaml
backgroundImage: "linear-gradient(to bottom, #1e3744, #301B29)"
```

Where to find gradients and colors:

- [Uigradients](https://uigradients.com/)
- [HappyHues](https://www.happyhues.co/)
