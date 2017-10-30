vertical padding between any elements, consistent across all email clients

eg. 15px
```html
<table width="100%">
    <tr>
      <td height="15" style="font-size: 15px; line-height: 15px;">&nbsp;</td>
    </tr>
</table>
```

also more consistent than using `<br>` or `style='padding-bottom:15px'` 


```html
<table width="100%">
    <tr>
        <td>
            <p class="h1">Hero text<p>
        </td>
    </tr>
    <tr>
        <td height="15" style="font-size: 15px; line-height: 15px;">&nbsp;</td>
    </tr>
    <tr>
        <td>
            <p>Copy text<p>
        </td>
    </tr>
</table>
```
