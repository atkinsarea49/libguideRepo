### Adding one or more Images in a Row (or with Captions)
This one is a little more complicated, but the images will align nicely with the captions. You can use this to either put multiple images in a row, add a caption to an image that conforms to the image's size, or both.
1. Copy and paste this code wherever you want your image(s) to be placed.
```
<div style="margin-left:auto !important; margin-right:auto !important; width:fit-content;">
	<div class="imagerow">
		<p>[PLACE IMAGE HERE]</p>
		<p class="caption">[PLACE CAPTION HERE]</p>
	</div>
</div>
```
2. You can increase the number of images that are placed next to each other by adding this code after the second to last `</div>` closing tag.
```
<div class="imagerow">
    <p>[PLACE IMAGE HERE]</p>
    <p class="caption">[PLACE CAPTION HERE]</p>
</div>
```
So if you had two images, it would look like this:
```
<div style="margin-left:auto !important; margin-right:auto !important; width:fit-content;">
	<div class="imagerow">
		<p>[PLACE IMAGE HERE]</p>
		<p class="caption">[PLACE CAPTION HERE]</p>
	</div>
	<div class="imagerow">
		<p>[PLACE IMAGE HERE]</p>
		<p class="caption">[PLACE CAPTION HERE]</p>
	</div>
</div>
```
3. Replace the indicated text **including the brackets**, but do not remove the quotes.
   - **[PLACE IMAGE HERE]** - Copy and paste your image element in between the `<p>` and `</p>` tags.
   - **[PLACE CAPTION HERE]** - Type your caption here.
4. Repeat for each image.
5. If you don't want the caption, delete this line:
```
<p class="caption">[PLACE CAPTION HERE]</p>
```
**Tip:** Images placed in these rows look best when they are all the same height. By default, libguides adds the width and height in a style attribute, which can be changed after-the-fact in the source code if necessary. For this, change the width to `auto` and the height to any number of pixels: `200px`. 200-300 is usually good. You can do this for every image in that row to make them line up nicely.
```
style="width: auto; height: 200px;"
```
