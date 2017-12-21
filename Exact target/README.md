Exact target, or ET sepertes the structure of the email from content the by using Templates and Data Extensions. 

Each Email is made up of modules

### PURPOSE

The Purpose section is the first section in the email - a bit like a hero - Newsletters and Plusmail's both have these, and they usully follow the same layout. Image, Header text, copy text and cta button

[example purpose](https://github.com/frc/email-resources-and-templates/blob/master/images/purpose.jpg)

|NAME|VALUE|
|---|---|
|PURPOSE heading|Escape to Asia|
|PURPOSE copy|Book flights to &lt;b&gt;Beijing&lt;/b&gt;, &lt;b&gt;Phuket&lt;/b&gt; or more in Asia|
|PURPOSE href|https://finnair.com/gb/gb?CAMPAIGN_ID=12345|
|PURPOSE image|http://image.email.finnair.com/lib/0d7c7d/m/3/GB_image.jpg|
|PURPOSE cta|Book now|
|PURPOSE color|#d7797d|
|PURPOSE utm|purpose+flights+to+asia+gb+newsletter|
|&nbsp;|&nbsp;|
|PURPOSE custom|some custom purpose module|
|custom field 1|some other button text|
|custom field 2|https://finnair.com/gb/gb?CAMPAIGN_ID=67890|
|custom field 3|purpose+other+destinations|

You can add color within the purpose copy like so `<b style='color:#0d1973'>Beijing</b>` if needed

The PURPOSE color value is optional, if blank the color of the heading and cta button will be finnair blue (#0d1973)

**new feature** Instead of having ALT purpose modules, you can create a new custom module to use instead of the normal purpose one. Just use the name of the module as the value for `PURPOSE custom` in the data extension. The new custom module can use PURPOSE heading, copy, href etc. **and** it can use custom fields as well, if needed.

---

### OFFERS BLOCK

The offers block contains 4 offers with an image and copy text like "Delhi from 789 €". If present, this block will normally come straight after the Purpose section

|NAME|VALUE|
|---|---|
|OFFERS BLOCK heading|Special offers to Italy|
|OFFERS BLOCK copy|Fly to &lt;b&gt;Rome&lt;/b&gt;, &lt;b&gt;Milan&lt;/b&gt; or other destinations in Italy...|
|OFFERS BLOCK href|https://finnair.com/gb/gb?CAMPAIGN_ID=12345|
|OFFERS BLOCK cta|Book now|
|OFFERS BLOCK color|#bada55|
|OFFERS BLOCK shape|diamond|
|OFFERS BLOCK personalise|true|
|OFFERS BLOCK utm|offers+block+flights+to+italy+gb+plusmail|
|&nbsp;|&nbsp;|
|OFFERS BLOCK 1|dest="ROM"|
|OFFERS BLOCK 2|dest="BKK" class="B"|
|OFFERS BLOCK 3|dest="VER" class="B" image="https://image-path.jpg" |
|OFFERS BLOCK 4|dest="NAP" utm="some+thing+else" price="789 €" |
|&nbsp;|&nbsp;|
|OFFERS BLOCK 1 replacement|ABC|
|OFFERS BLOCK 2 replacement|DEF&vert;biz|
|OFFERS BLOCK 3 replacement|GHI|
|OFFERS BLOCK 4 replacement|JKL|

`OFFERS BLOCK heading`, `copy`, `cta`, `color`, `shape` and `personalise` are optional, and can be left blank. replacement offers are also optional

You only need to pass the 3-letter airport code for each individual offer, and ET will generate the destination name, price, and href from the offers json feed [example](https://api.finnair.com/v1/offerfeed/offers?locale=fi_FI). It will also generate the image and utm 

Adding `class="B"` after the 3-digit airport code will fetch the business class offer (default economy, if blank)

Adding `price="123 €"` will pass this price instead of using the offers feed price

Adding `image="https://finnair.com/go/some-image.jpg"` will use a custom image, instead of the default ones [found here](https://www.finnair.com/go/responsive/Images/newsletters/300x300_destination/ROM.jpg)

Adding `color="#d7797d"` will pass a custom color for the price

Adding `href="https://finnair.com/some-custom-link"` will pass a custom link for the offer instead of using [these](https://www.finnair.com/fi/gb/offers?OFFER_ID=4200)


If a replacement offer is declared then ET will check if the user has a future booking (up to a month) to one of the original 4 destinations, and replace it with the replacement offer. (It will also check the replacement offers, so that it doesn't use a the replacement offer if a user has also booked a flight to one of them). Same rules for customizing apply

---

### OFFERS TABLE

The offers table will show a list of up to 12 offers in a simple table, the table can have one or two columns, and can be customized by color


|NAME|VALUE|
|---|---|
|OFFERS TABLE columns|2|
|OFFERS TABLE heading|Our latest offers to Asia|
|OFFERS TABLE copy|Book flights to Beijing, Phuket or elsewhere in Asia...|
|OFFERS TABLE color|#c0ffee|
|OFFERS TABLE cta|See all offers|
|OFFERS TABLE href|https://finnair.com/some-link|
|OFFERS TABLE utm|some+utm+stuff|
|&nbsp;|&nbsp;|
|OFFERS TABLE col 1 color|#f00f00|
|OFFERS TABLE col 1 heading|Economy class offers|
|OFFERS TABLE col 1 subheading left|Destination|
|OFFERS TABLE col 1 subheading right|Return from|
|OFFERS TABLE col 1 personalize|true|
|OFFERS TABLE col 1 cta|See all economy offers to Asia|
|OFFERS TABLE col 1 href|https://finnair.com/some-link|
|OFFERS TABLE col 1 utm|some+utm+stuff|
|&nbsp;|&nbsp;|
|OFFERS TABLE col 2 color|#b00b00|
|OFFERS TABLE col 2 heading|Business class offers|
|OFFERS TABLE col 2 subheading left|Destination|
|OFFERS TABLE col 2 subheading right|Return from|
|OFFERS TABLE col 2 personalize|true|
|OFFERS TABLE col 2 cta|See all business offers to Asia|
|OFFERS TABLE col 2 href|https://finnair.com/some-link|
|OFFERS TABLE col 2 utm|some+utm+stuff|
|&nbsp;|&nbsp;|
|OFFERS TABLE col 1 offer 1|BJS|
|OFFERS TABLE col 1 offer 2|CAN|
|OFFERS TABLE col 1 offer 3|GZN|
|OFFERS TABLE col 1 offer 4|PVG|
|OFFERS TABLE col 1 offer 5|XIY|
|&nbsp;|&nbsp;|
|OFFERS TABLE col 2 offer 1|BJS&vert;biz|
|OFFERS TABLE col 2 offer 2|CAN&vert;biz|
|OFFERS TABLE col 2 offer 3|GZN&vert;biz|
|OFFERS TABLE col 2 offer 4|PVG&vert;biz|
|OFFERS TABLE col 2 offer 5|XIY&vert;biz|
|&nbsp;|&nbsp;|
|OFFERS TABLE col 1 replacement 1|ABC|
|OFFERS TABLE col 1 replacement 2|DEF|
|&nbsp;|&nbsp;|
|OFFERS TABLE col 2 replacement 1|ABC&vert;biz|
|OFFERS TABLE col 2 replacement 2|DEF&vert;biz|

Table offers can be customized the same way that block offers can be (but no image), eg.

`BCN|{399 €}|#abc123|https://www.finnair.com/some-link`

###### the color must be a 6-digit hex code and the price must be inside brackets `{}`

All headings, subheadings and cta's are optional

---

### PREMIUMS

Premiums are generally 3rd party offers/adverts that come under the offers table. They have two equal columns, image-text (sales letters), or text-image (plusmail). There can be up to 12 premiums

|NAME|VALUE|
|---|---|
|PREMIUM 1 heading|Rent a car from Hertz|
|PREMIUM 1 copy|Rent a car from 100's of destinations using Hertz...|
|PREMIUM 1 href|https://finnair.com/gb/gb/rent-a-car|
|PREMIUM 1 image|http://image.email.finnair.com/lib/0d7c7d/m/3/hertz.jpg|
|PREMIUM 1 cta|Read more|
|PREMIUM 1 order|text-image|
|PREMIUM 1 color|#d7797d|
|PREMIUM 1 utm|premium+rent+a+car+hertz+gb+newsletter|
|&nbsp;|&nbsp;|
|PREMIUM 1 custom|some custom premium module|
|custom field 5|An extra headline|
|custom field 6|a bunch of extra copy text for you to read|

`PREMIUM order` defines how the premium looks on desktop. On mobile the image will always be above the text

`text-image` text on the left - image on the right

`image-text` image on the left - text on the right (default, will be used if blank also)


**new feature** Instead of having ALT premium modules, you can create a new custom module to use instead of the normal premium one. Just use the name of the module as the value for `PREMIUM x custom` in the data extension. (x is the number of the premium) The new custom module can use PREMIUM heading, copy, href etc. **and** it can use custom fields as well, if needed. (same as custom purpose modules)
