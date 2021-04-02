# jupyter notebook auto dark mode

The `custom.css` auto change the background color and text color.

inspire by jupyter-themes

### Usage

```bash
git clone --depth=1 https://github.com/toyourheart163/jupyter-auto-dark-mode
cd jupy[tab]
mv ~/.jupyter/custom/custom.css{,pre}  # backup
mkdir -p ~/.jupyter/custom
cp custom.css ~/.jupyter/custom/
```

### How

```css
:root {}
@media (prefers-color-scheme: dark) {
  :root {
    --background-color: #1e1f23;
  }
}

/* auto change color */
body {
  var(--background-color)
}
```
