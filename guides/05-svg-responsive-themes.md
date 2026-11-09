# 05 — SVG, themes, and responsive layouts

SVGs can make banners crisp at different screen sizes, but accessibility and readability come first.

For theme-aware images, GitHub supports a `<picture>` pattern with light/dark sources:

```html
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="../assets/banner-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="../assets/banner-light.svg">
  <img alt="GitHub Profile Design Studio workshop banner" src="../assets/banner-light.svg">
</picture>
```

When copying this pattern into **your profile repository**, update the image paths to match the assets you have copied there. Relative paths are relative to the README's location.

Avoid embedding scripts, relying on unsupported CSS, or using tiny text baked into banners. Always check mobile widths and both themes.
