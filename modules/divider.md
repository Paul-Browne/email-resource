##### full width divider, like `<hr>`

```html
<table width="100%">                    
    <tr>
        <td style="border-bottom:1px solid #ddd;"></td>
    </tr>
</table>
```

##### divider with padding

```html
<table width="100%">
    <tr>
        <td class="inner contents">            
            <table width="100%">                    
                <tr>
                    <td style="border-bottom:1px solid #ddd;"></td>
                </tr>
            </table> 
        </td>
    </tr>
</table>  
```

##### divider with padding and small logo in middle

```html
<table width="100%">
    <tr>
        <td class="inner contents">            
            <table width="100%">                    
                <tr>
                    <td style="border-bottom:1px solid #ddd;"></td>
                    <td style="font-size:0;text-align:center; vertical-align: middle;" width="100">
                        <img src="https://sunshine.finnair.com/assets/img/f-logo-blue.png" alt="Finnair" width="77" border="0">
                    </td>
                    <td style="border-bottom:1px solid #ddd;"></td>        
                </tr>
            </table> 
        </td>
    </tr>
</table>
```

![divider with logo](https://github.com/frc/email-resources-and-templates/blob/master/images/divider-with-logo.jpg)
