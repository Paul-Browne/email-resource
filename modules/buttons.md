####Buttons

don't ask why the button markup is dozens of lines, it just is.
color change `background: #0d1974`
radius change `background-radius: 3px`
href change *all* the `href`s

######TODO 
add smaller button

#####button

```html
<table align="center" border="0" cellpadding="0" cellspacing="0" width="100%">
  <tr>
    <td>
      <table align="left" cellpadding="0" cellspacing="0" style="border-radius:3px; background: #0d1974;">
        <tr>
          <td height="40" width="10">
            <a style="display: block; height: 40px; line-height: 40px; color: #ffffff; text-decoration: none; text-transform: uppercase; font-size: 16px;" href="https://www.finnair.com">&nbsp;</a>
          </td>
          <td height="40" style="font-family: Helvetica, Arial, Sans-serif;">
              <a style="display: block; height: 40px; line-height: 40px; color: #ffffff; text-decoration: none; text-transform: uppercase; font-size: 16px;" href="https://www.finnair.com">READ MORE</a>
          </td>
          <td height="40" width="10">
            <a style="display: block; height: 40px; line-height: 40px; color: #ffffff; text-decoration: none; text-transform: uppercase; font-size: 16px;" href="https://www.finnair.com">&nbsp;</a>
          </td>
        </tr>
      </table>
    </td>
  </tr>
</table>
```

#####fixed width button

change `width="150"` to the desired width

```html
<table align="center" border="0" cellpadding="0" cellspacing="0" width="100%">
  <tr>
    <td>
      <table align="left" cellpadding="0" cellspacing="0" style="border-radius:3px; background: #0d1974;">
        <tr>
          <td height="40" width="150" style="font-family: Helvetica, Arial, Sans-serif;">
              <a style="display: block; height: 40px; line-height: 40px; color: #ffffff; text-decoration: none; text-transform: uppercase; font-size: 16px; text-align: center" href="https://www.finnair.com">READ MORE</a>
          </td>
        </tr>
      </table>
    </td>
  </tr>
</table>
```

#####button with arrow

```html
<table align="center" border="0" cellpadding="0" cellspacing="0" width="100%">
  <tr>
    <td>
      <table align="left" cellpadding="0" cellspacing="0" style="border-radius:3px; background: #0d1974;">
        <tr>
          <td height="40" width="10">
            <a style="display: block; height: 40px; line-height: 40px; color: #ffffff; text-decoration: none; text-transform: uppercase; font-size: 16px;" href="https://www.finnair.com">&nbsp;</a>
          </td>
          <td height="40" style="font-family: Helvetica, Arial, Sans-serif;">
              <a style="display: block; height: 40px; line-height: 40px; color: #ffffff; text-decoration: none; text-transform: uppercase; font-size: 16px;" href="https://www.finnair.com">READ MORE</a>
          </td>
          <td height="40" width="10">
            <a style="display: block; height: 40px; line-height: 40px; color: #ffffff; text-decoration: none; text-transform: uppercase; font-size: 16px;" href="https://www.finnair.com">&nbsp;</a>
          </td>
          <td height="40" style="font-size:0;">
            <a style="display: block; height: 40px;" href="https://www.finnair.com">
              <img height="18" style="padding-top: 11px; vertical-align: middle; display: block;" src="http://image.email.finnair.com/lib/fe92127276640d7c7d/m/2/new_arrow_right.png">
            </a>
          </td>
          <td height="40" width="10">
            <a style="display: block; height: 40px; line-height: 40px; color: #ffffff; text-decoration: none; text-transform: uppercase; font-size: 16px;" href="https://www.finnair.com">&nbsp;</a>
          </td>
        </tr>
      </table>
    </td>
  </tr>
</table>
```

#####fixed width button with arrow

```html
<table align="center" border="0" cellpadding="0" cellspacing="0" width="100%">
  <tr>
    <td>
      <table align="left" cellpadding="0" cellspacing="0" style="border-radius:3px; background: #0d1974;">
        <tr>
          <td height="40" width="10">
            <a style="display: block; height: 40px; line-height: 40px; color: #ffffff; text-decoration: none; text-transform: uppercase; font-size: 16px;" href="https://www.finnair.com">&nbsp;</a>
          </td>
          <td height="40" width="150" style="font-family: Helvetica, Arial, Sans-serif;">
              <a style="display: block; height: 40px; line-height: 40px; color: #ffffff; text-decoration: none; text-transform: uppercase; font-size: 16px;" href="https://www.finnair.com">READ MORE</a>
          </td>
          <td height="40" width="10">
            <a style="display: block; height: 40px; line-height: 40px; color: #ffffff; text-decoration: none; text-transform: uppercase; font-size: 16px;" href="https://www.finnair.com">&nbsp;</a>
          </td>
          <td height="40" style="font-size:0;">
            <a style="display: block; height: 40px;" href="https://www.finnair.com">
              <img height="18" style="padding-top: 11px; vertical-align: middle; display: block;" src="http://image.email.finnair.com/lib/fe92127276640d7c7d/m/2/new_arrow_right.png">
            </a>
          </td>
          <td height="40" width="10">
            <a style="display: block; height: 40px; line-height: 40px; color: #ffffff; text-decoration: none; text-transform: uppercase; font-size: 16px;" href="https://www.finnair.com">&nbsp;</a>
          </td>
        </tr>
      </table>
    </td>
  </tr>
</table>
```