# Seek-and-Find Pages
## Base Code
These should be unlisted but public. You can add listings for items (such as the spiders) by following these instructions:
1. Copy the following code to wherever you want the listings to be. This configuration has two "slots."
```
<div class="flexcontainer">

	<div class="flexbox">
		<div class="[RARITY] found-item-div">
			<p>[INSERT NAME HERE]</p>
			<p><img alt="" class="found-item-img" loading="lazy" src="[PASTE LINK TO IMAGE HERE]" /></p>
			<p>Interested in learning more?</p>
			<ul>
				<li><a href = "[URL OF RESOURCE]">[NAME OF RESOURCE]</a></li>
				<li><a href = "[URL OF RESOURCE]">[NAME OF RESOURCE]</a></li>
			</ul>
		</div>
	</div>

	<div class="flexbox">
		<div class="[RARITY] found-item-div">
			<p>[INSERT NAME HERE]</p>
			<p><img alt="" class="found-item-img" loading="lazy" src="[PASTE LINK TO IMAGE HERE]" /></p>
		</div>
	</div>

</div>
```


- [INSERT NAME HERE] - put the name of the item here
- [PASTE LINK TO IMAGE HERE] - paste the link to your image here. Make sure to include the quotes.
- [RARITY] - See below
- [URL OF RESOURCE] - paste the link to a resource where students can learn more information
- [NAME OF RESOURCE] - put the name of the resource here.
	- You can add more resources to this list by adding more of these lines:
		
```
<li><a href = "[URL OF RESOURCE]">[NAME OF RESOURCE]</a></li>
```

2. You can add more "slots" by pasting this code before the last tag, one for each item:
```
<div class="flexbox">
		<div class="[RARITY] found-item-div">
			<p>[INSERT NAME HERE]</p>
			<p><img alt="" class="found-item-img" loading="lazy" src="[PASTE LINK TO IMAGE HERE]" /></p>
		</div>
	</div>
```
## Changing Border Color Based on Rarity
There are several rarity types. Each one has a dedicated border color. Designate the item's rarity by pasting the cooresponding name in place of [RARITY] in the base code. These are the available rarities. Copy and paste the name directly.
- `common-div` - Common rarity
- `rare-div` - Rare rarity 
- `sr-div` - Super Rare rarity
- `ur-div` - Ultra Rare rarity
### Example
For a common item, the line would look like this:
```
<div class="common-div found-item-div">
```
