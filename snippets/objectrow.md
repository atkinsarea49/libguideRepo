## Placing Two Objects Next to Each Other
Yeah, you can do this natively, sort of. This will make it look nice and will center the smaller element. Plus, you're not just limited to pictures next to text. Also, why use float when you can use flex.
1. To use this, paste the following code:
```
<div class="flexcontainer">
	<div class="flexbox">
		[YOUR ITEM HERE]
	</div>
	<div class="flexbox">
		[YOUR ITEM HERE]
	</div>
</div>

```
2. Replace both appearances of `[YOUR ITEM HERE]` with whatever you want your content to be. It can be a `<p>`, an `<img>`, etc.
3. Important Note: Libguides will natively hard-code the size of your image. This does not have a negative effect on desktop, but it looks really bad on mobile. So if you are using images, be sure to remove the following from the code in the `<img>` tag:
```
style="width: 300px; height: 300px;"
```
4. The actual numbers used for the dimensions may vary.
