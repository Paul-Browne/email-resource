##### four column layout

four columns on desktop

two columns on mobile

Four column layout, columns content is only 140px wide, 160px minus 20px of padding (10px either side). It is possible to decrease the padding by replacing the class `inner` with `inner5`, or you can increase the padding by using `inner20`

[four columns](https://github.com/frc/email-resources-and-templates/blob/master/images/four%20columns.jpg)
[four columns mobile](https://github.com/frc/email-resources-and-templates/blob/master/images/four%20columns%20mobile.jpg)

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
                        <td class="four-column">
                            <!--[if (gte mso 9)|(IE)]>
                            <table width="100%">
                            <tr>
                            <td width="50%" valign="top">
                            <![endif]-->
                            <div class="column">
                                <table width="100%">
                                    <tr>
                                        <td class="inner contents">
                                            <!-- contents -->
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
                                            <!-- contents -->
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
            </div>
            <!--[if (gte mso 9)|(IE)]>
            </td><td width="50%" valign="top">
            <![endif]-->
            <div class="column">
                <table width="100%">
                    <tr>
                        <td class="four-column">
                            <!--[if (gte mso 9)|(IE)]>
                            <table width="100%">
                            <tr>
                            <td width="50%" valign="top">
                            <![endif]-->
                            <div class="column">
                                <table width="100%">
                                    <tr>
                                        <td class="inner contents">
                                            <!-- contents -->
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
                                            <!-- contents -->
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
