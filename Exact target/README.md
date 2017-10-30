Exact target, or ET sepertes the structure of the email from content the by using Templates and Data Extensions. 

Each Email is made up of modules

### PURPOSE

The Purpose section is the first section in the email - a bit like a hero - Newsletters and Plusmail's both have these, and they usully follow the same layout. Image, Header text, copy text and cta button

[example purpose](https://github.com/frc/email-resources-and-templates/blob/master/images/purpose.jpg)

|NAME|VALUE|
|---|---|
|PURPOSE heading|Escape to Asia|
|PURPOSE copy|Book flights to &lt;b&gt;Beijing&lt;/b&gt;, &lt;b&gt;Phuket&lt;/b&gt; or other exciting destinations in Asia...|
|PURPOSE href|https://finnair.com/gb/gb?CAMPAIGN_ID=12345|
|PURPOSE image|http://image.email.finnair.com/lib/0d7c7d/m/3/GB_image.jpg|
|PURPOSE cta|Book now|
|PURPOSE color|#d7797d|
|PURPOSE utm|purpose+flights+to+asia+gb+newsletter|

You can add color within the purpose copy like so `<b style='color:#0d1973'>Beijing</b>` if needed

The PURPOSE color value is optional, if blank the color of the heading and cta button will be finnair blue (#0d1973)

---

### OFFERS BLOCK

The offers block contains 4 offers with an image and copy text like "Delhi from 789 €"

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
|OFFERS BLOCK 1|ROM|
|OFFERS BLOCK 2|MIL&vert;biz|
|OFFERS BLOCK 3|VER|
|OFFERS BLOCK 4|NAP|
|OFFERS BLOCK 1 replacement|ABC|
|OFFERS BLOCK 2 replacement|DEF&vert;biz|
|OFFERS BLOCK 3 replacement|GHI|
|OFFERS BLOCK 4 replacement|JKL|

`OFFERS BLOCK heading`, `copy`, `cta`, `color`, `shape` and `personalise` are optional, and can be left blank. replacement offers are also optional

You only need to pass the 3-letter airport code for each individual offer, and ET will generate the destination name, price, href, image and utm from the offers page data ext. `Shared Items > Shared Data Extensions > __offers page`

Adding `biz` after the 3-digit airport code will fetch the business class offer (default economy, if blank)

It is possible to use a custom color, price, image or href for an offer like so

`DEL|#123123|{499 €}|finnair.com/custom-image.jpg|https://finnair.com/gb/gb/some-custom-page`

###### the color must be a 6-digit hex code, the price must be inside brackets `{}` and the image must be either a .jpg or .png

If a replacement offer is declared then ET will check if the user has a future booking (up to a month) to one of the original 4 destinations, and replace it with the replacement offer. (It will also check the replacement offers, so that it doesn't use a the replacement offer if a user has also booked a flight to one of them)
