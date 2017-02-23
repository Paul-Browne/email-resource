#####email base html

```html
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
<html xmlns="http://www.w3.org/1999/xhtml">
<head>
<meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
    <!--[if !mso]><!-->
        <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <!--<![endif]-->
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title></title>
    <!--[if (gte mso 9)|(IE)]>
    <style type="text/css">
        table {border-collapse: collapse;}
    </style>
    <![endif]-->
    <style>
        /* Basics */
        body {
            margin: 0 !important;
            padding: 0;
            background-color: #ffffff;
        }
        table {
            border-spacing: 0;
            font-family: sans-serif;
            color: #333333;
        }
        td {
            padding: 0;
        }
        img {
            border: 0;
            vertical-align: middle;
        }
        div[style*="margin: 16px 0"] { 
            margin:0 !important;
        }
        .wrapper {
            width: 100%;
            table-layout: fixed;
            -webkit-text-size-adjust: 100%;
            -ms-text-size-adjust: 100%;
        }
        .webkit {
            max-width: 640px;
            margin: 0 auto;
        }
        .outer {
            Margin: 0 auto;
            width: 100%;
            max-width: 640px;
        }     
        .full-width-image img {
            width: 100%;
            max-width: 640px;
            height: auto;
        }
        .inner {
            padding-left: 10px;
            padding-right: 10px;
        }
        p {
            Margin: 0;
            font-size: 14px;
        }
	    a, a:visited {
	        color: #0d1974;
	        text-decoration: underline;
	    }
        .h1 {
            font-size: 24px!important;
            font-weight: bold;            
        }
        .h2 {
            font-size: 21px!important;
            font-weight: bold;            
        }
         
        /*Two column layout*/
        .two-column {
            text-align: center;
            font-size: 0;
        }
        .two-column .column {
            width: 100%;
            max-width: 320px;
            display: inline-block;
            vertical-align: top;
        }
        .contents {
            width: 100%;
        }
        .two-column .contents {
            font-size: 14px;
            text-align: left;
        }
        .two-column img {
            width: 100%;
            max-width: 300px;
            height: auto;
        }
        @media only screen and (max-width:440px) {
            .two-column .column,
            .two-column img{
                max-width: none!important;
            }       
        }

        @media yahoo {
            .two-column .column {
                float: left;
            }
            .two-column.rtl .column {
                float: right;           
            }       
        }  
    </style>
</head>

<!--

full width image
======== 640 ========

one-column
=|=================|=
10       620      10

two-column
=|=======|=|=======|=
10  300  20   300  10

-->

<body>
    <center class="wrapper">
        <div class="webkit">
            <!--[if (gte mso 9)|(IE)]>
            <table cellpadding="0" cellspacing="0" border="0" width="640" align="center">
            <tr>
            <td>
            <![endif]-->
            <table class="outer" align="center">
                <tr>
                    <td>
    
                        <!-- ALL THE CONTENT GOES HERE-->

                    </td>
                </tr>
            </table>
            <!--[if (gte mso 9)|(IE)]>
            </td>
            </tr>
            </table>
            <![endif]-->
        </div>
    </center>
</body>
</html>
```