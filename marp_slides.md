---
marp: true
author: Petr Ankudinov
theme: default
class: invert
backgroundImage: "linear-gradient(to bottom, #1e3744, #301B29)"
# backgroundImage: "linear-gradient(to right, #0f2027, #203a43, #2c5364)"
# backgroundImage: "linear-gradient(to bottom, #004643, #001e1d)"
paginate: true
style: |
  footer {
    font-size: 14px
  }
  section::after {
    font-family: Brush Script MT;
    font-size: 14px;
  }
  pre {
    background: linear-gradient(to top, #1e3744, #301B29);
  }

---
# How to Build Marp Slides

<!-- Do not add page number on this slide -->
<!--
_paginate: false
-->

```json
{
  "date": "12.04.2024",
  "topic": "random things about marp",
  "author": "Petr Ankudinov"
}
```

![bg right](img/pexels-renato-rocca-9279669.jpg)

---

<!-- Add footer starting from this slide -->
<!--
footer: April 2024
-->

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

---

# How To Use Animated Images

- This looks amazing on a starting page

```markdown
![bg right fit](https://github.com/srl-labs/containerlab/raw/main/docs/images/containerlab_export_white_ink.svg?sanitize=true)
```

![bg right fit](https://github.com/srl-labs/containerlab/raw/main/docs/images/containerlab_export_white_ink.svg?sanitize=true)

---

# Using List

```markdown
- item1
- item2
```

- item1
- item2

---

# Animated List

- Some Item

  - subitem

* This will be hidden at first

```markdown
- Some Item

  - subitem

* This will be hidden at first
```

---

# Paginate

```markdown
---
paginate: true

---
<!-- Do not add page number on this slide -->
<!--
_paginate: false
-->

```

---

# Footer

```markdown
<!-- Add footer starting from this slide -->
<!--
footer: 'April 2024'
-->

```

---

# Add Image as Footer

```markdown
<!-- Add footer starting from this slide -->
<!--
footer: '![h:20](https://www.arista.com/assets/images/logo/Arista_Logo.png)'
-->
```
