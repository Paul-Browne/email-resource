Add this at the end of the global `style` in the `head` You only need to declare the `woff` format, since all the clients that allow the `@font-face` attribute accept the `woff` format.

#### Self hosted fonts

```css
@font-face {
    font-family: 'custom font';
    src: url('https://www.example.com/path/to/custom/font.woff') format('woff');
    font-weight: normal;
    font-style: normal;
}
@media screen {
    .custom-font {
        font-family: 'custom font', Helvetica, Arial, Sans-serif;
    }
}
```

#### Externally sourced fonts (eg. google fonts)

```html
<link href="https://fonts.googleapis.com/css?family=Libre+Baskerville:400,400i,700" rel="stylesheet">
```

```css
@media screen {
    .custom-font {
        font-family: 'Libre Baskerville', serif;
    }
}
```

The reason you need to place the `.custom-font` inside the `@media screen` query is that Outlook doesn't accept custom fonts and will always fallback to times new roman, even if you declare Helvetica, Arial or Sans-serif in the font stack. But since Outlook also ignores anything inside a `@media` query, the custom font stack will be ignored
