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
  .columns {
      display: grid;
      grid-template-columns: repeat(2, minmax(0, 1fr));
      gap: 1rem;
  }
  .columns3 {
    display: grid;
    grid-template-columns: repeat(3, minmax(0, 1fr));
    gap: 1rem;
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

<style scoped>section {font-size: 24px;}</style>

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

---

# 2 Columns

<div class="columns">
<div>

- test
- test

</div>
<div>

```json
{
  "a": 1,
  "b": 2
}
```

</div>

---

# 3 columns

<div class="columns3">
<div>

- test
- test

</div>
<div>

abc

</div>
<div>

![h:300 sepia](img/pexels-adrien-olichon-2823459.jpg)

</div>
</div>

---

# Font Size

<style scoped>section {font-size: 14px;}</style>

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus hendrerit aliquet sem a faucibus. Nam et viverra purus. Duis quis fringilla libero. Duis et tortor pharetra leo bibendum mollis. Integer vel felis lectus. Phasellus varius placerat facilisis. Phasellus placerat orci quis eros elementum ornare. Proin quis odio eu lorem gravida condimentum nec vel nisi. Pellentesque euismod est eget pharetra rhoncus. Donec eget consectetur nibh, ut fringilla nisl. Nulla facilisi.

Maecenas sit amet egestas magna. Suspendisse aliquet eget ligula non suscipit. Suspendisse pulvinar blandit commodo. Suspendisse malesuada venenatis ullamcorper. In hac habitasse platea dictumst. Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia curae; Interdum et malesuada fames ac ante ipsum primis in faucibus. Pellentesque a erat quis neque sodales hendrerit ac non nibh. Nunc tempus porta lectus, eu eleifend neque blandit quis.

Duis at lorem dolor. Praesent in auctor augue. Suspendisse pharetra suscipit leo, vel ornare diam consectetur in. Nunc vestibulum diam rhoncus tellus ultricies rhoncus. Curabitur hendrerit vel purus vitae ultrices. Vestibulum efficitur elit eget pharetra congue. Aenean porta mauris pellentesque lacus malesuada, eget iaculis justo laoreet. Ut justo elit, rutrum sed varius at, bibendum non libero. Fusce auctor quam nec urna euismod, at egestas nulla posuere. Phasellus ac nunc nec nibh porttitor malesuada sit amet sit amet enim. Donec venenatis laoreet pretium. Vestibulum metus sapien, molestie a arcu eget, tempor blandit lectus.

Donec dapibus sapien et volutpat iaculis. Quisque tincidunt nunc a diam posuere convallis. Donec ut volutpat ipsum. Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. Cras posuere dui quis mattis varius. Praesent auctor sem vel lacinia posuere. Fusce posuere eget erat non gravida. Nunc eu justo quam. Etiam sit amet mollis turpis. Sed vitae rutrum lectus. Proin ut lobortis ante. Nam varius posuere enim non tristique. Praesent facilisis malesuada orci nec feugiat. In eget ex eget ipsum pretium tincidunt. Etiam mollis tellus eu fermentum tempus.

Ut semper, ipsum in consequat rutrum, mauris quam efficitur sem, vitae volutpat quam nunc eget dolor. Cras facilisis eros quis nisl porta, non tincidunt felis placerat. Aliquam non luctus lorem. Aenean euismod ut leo at ornare. Vivamus non porttitor eros. Mauris ante libero, rutrum ut massa sed, ornare sollicitudin elit. Fusce ut iaculis velit. Morbi a ultrices odio. Sed faucibus porttitor erat sed congue. Sed ornare posuere felis eu suscipit. Suspendisse tempor lorem sed tortor laoreet condimentum. Cras sit amet urna id eros faucibus ultricies sed sed magna. Proin quis erat a turpis lobortis viverra. Curabitur in mollis eros.
