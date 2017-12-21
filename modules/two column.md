### image-text
two columns on desktop: image on the left, text on the right

one column on mobile: image above text

```html
<table width="100%">
    <tr>
        <td class="two-column">
            <!--[if (gte mso 9)|(IE)]>
            <table width="100%">
            <tr>
            <td width="50%" valign="top">
            <![endif]-->
            <div class="column">
                <table width="100%">
                    <tr>
                        <td class="inner contents">
                            <img src="http://placekitten.com/g/310/310" width="300" alt="" />
                        </td>
                    </tr>
                </table>
            </div>
            <!--[if (gte mso 9)|(IE)]>
            </td><td width="50%" valign="top">
            <![endif]-->
            <div class="column">
                <table width="100%">
                    <tr>
                        <td class="inner contents">
                            <p class="h1">Lorem ipsum dolor sit amet</p>
                            <table border="0" cellspacing="0" cellpadding="0" align="center" width="100%">
                                <tr>
                                  <td height="15" style="font-size: 15px; line-height: 15px;">&nbsp;</td>
                                </tr>
                            </table>
                            <p>Maecenas sed ante pellentesque, posuere leo id, eleifend dolor. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos. Praesent laoreet malesuada cursus. Maecenas scelerisque congue eros eu posuere. Praesent in felis ut velit pretium lobortis rhoncus ut erat.</p>
                        </td>
                    </tr>
                </table>
            </div>
            <!--[if (gte mso 9)|(IE)]>
            </td>
            </tr>
            </table>
            <![endif]-->
        </td>
    </tr>
</table>
```
![image-text](https://github.com/frc/email-resources-and-templates/blob/master/images/image-text.jpg)

![two columns mobile](https://github.com/frc/email-resources-and-templates/blob/master/images/two%20column%20mobile.jpg)

### text-image
two columns on desktop: text on the left, image on the right

one column on mobile: image above text

using `dir="rtl"` it is possible to reverse the order of the columns for desktop, but maintining the same image above text layout for mobile

```html
<table width="100%">
    <tr>
        <td class="two-column rtl" dir="rtl">
            <!--[if (gte mso 9)|(IE)]>
            <table width="100%" dir="rtl">
            <tr>
            <td width="50%" valign="top">
            <![endif]-->
            <div class="column" dir="ltr">
                <table width="100%">
                    <tr>
                        <td class="inner contents">
                            <img src="http://placekitten.com/g/310/310" width="300" alt="" />
                        </td>
                    </tr>
                </table>
            </div>
            <!--[if (gte mso 9)|(IE)]>
            </td><td width="50%" valign="top">
            <![endif]-->
            <div class="column" dir="ltr">
                <table width="100%">
                    <tr>
                        <td class="inner contents">
                            <p class="h1">Lorem ipsum dolor sit amet</p>
                            <table border="0" cellspacing="0" cellpadding="0" align="center" width="100%">
                                <tr>
                                  <td height="15" style="font-size: 15px; line-height: 15px;">&nbsp;</td>
                                </tr>
                            </table>
                            <p>Maecenas sed ante pellentesque, posuere leo id, eleifend dolor. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos. Praesent laoreet malesuada cursus. Maecenas scelerisque congue eros eu posuere. Praesent in felis ut velit pretium lobortis rhoncus ut erat.</p>
                        </td>
                    </tr>
                </table>
            </div>
            <!--[if (gte mso 9)|(IE)]>
            </td>
            </tr>
            </table>
            <![endif]-->
        </td>
    </tr>
</table>
```
![text-image](https://github.com/frc/email-resources-and-templates/blob/master/images/text-image.jpg)
