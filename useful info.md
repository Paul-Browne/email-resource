## Dont's

Dont use `<h1>, <h2> or <h3>` elements, they style inconsistently across email clients

Instead use `<p class="h1">`

---

Don't use **padding** or **margin** on `<a>` or `<span>`, or any inline element. Even if you add `display:block` the padding still won't be applied, since you can't change an elements `display` attribute in Outlook

Instead wrap the `<a>` in a table and add the padding to the `<td>`

```html
<table width="100%">
  <tr>
    <td style='padding:10px'>
      <a href="some-link">some text</a>
    </td>
  </tr>
</table>
```
