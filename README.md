# A49 Libguide Custom Code Documentation
Here's how to use the custom code stuff I made for our libguide!
# Linking external CSS File
For any of this to work or look even remotely good, you need to copy and paste a reference to this custom CSS into your libguide's Custom CSS/JS Box.

To find this box:
1. On the editing page for your libguide, find and click on the Look and Feel Icon, then Click "Guide Custom CSS/JS."
![screenshot of the look and feel menu open. the guide custom css/js option is highlighted in red](documentationImages/customCss1.png)
2. Paste the following code:
```
<link rel="stylesheet" type="text/css" href="https://bstensonwork.github.io/libguideRepo/libguideCSS.css">
```
# Adding Custom Elements
Most of these techniques require you to edit the source code for your content items. In the rich text editing window, click the "Source" icon. This will show you the bare (and horribly linted) HTML. It can look a little all over the place, so here are some general tips for reading it.
- Most HTML elements have an opening and closing tag that tells the computer where the element starts and begins. These tags look like this:
```
<p>Your content here!</p>
```
- Notice how the closing tag has a `/` before the element's name.
- You can nest multiple elements inside each other.
- 
- Some elements like images only have a singular tag, which looks like this:
```
<img href="blahblahblah.com/image" alt="Alternate text" />
```
- Notice that instead of a closing tag, this image element has a `/>` at the end.
- This element also has attributes (`href="blahblahblah.com/image"` and `alt="Alternate text"`), which are little bits of text that tell the computer how to display the element. These are usually in the opening tag.
- [Read more about HTML elements here](https://www.w3schools.com/html/html_elements.asp)
## Details Dropdown
This element will put a question mark icon wherever you paste the code that opens a collapsing box for images/more details/explanations/etc. It looks best when placed at the end of a line. It is classed as a button and styled to look a little better inline.
![Screenshot of a green question mark button at the end of a line](documentationImages/detailsDropdown1.png)
![Screenshot of an opened collapsable box underneath the line from the above image. The question mark icon is gold to indicate that the box has been opened](documentationImages/detailsDropdown2.png)
1. Copy and paste the following code at the end of a text element like `<p>` (paragraph) or `<li>` (list item). You can also put these at the end of headings like `<h2>` or `<h3>`. Paste the code **before** the closing tag (the tag with the `/` before the name, such as `</p>` or `</h3>`.
```
<button aria-controls="[ID HERE]" aria-expanded="false" aria-label="[LABEL HERE]" class="btn btn-default question-btn" data-toggle="collapse" href="#[ID HERE]" title="[TOOLTIP HERE]">
    <span class="glyphicon glyphicon-question-sign"></span>
</button>
<div class="collapseBox collapse" id="[ID HERE]">
   <p>[PLACE YOUR CONTENT HERE]</p>
</div>
```
2. You will need to replace several things in this code. Replace the following text **including the brackets**
  - **[ID HERE]** - This should be a unique identifier for your dropdown box. All lowercase, use hyphens instead of spaces, no special characters.
    - e.g. `aria controls="simple-mode-explanation"`
    - e.g. `href="#simple-mode-explanation"`
      - Note: the href needs to have the `#`, so be sure to leave that be when filling this in.
    - e.g. `id="simple-mode-explanation"`
  - **[LABEL HERE]** - This is an Aria label, which is what a screen reader will read aloud when the user selects the button. Try to use something descriptive but short. Use spaces in this one, but limit special characters.
    - e.g. `aria-label="Simple mode explanation"`
  - **[TOOLTIP HERE]** - This is the little tiny text that pops up when you hover over an element. This is usually not seen by screen readers or mobile users, so it's best not to put any essential information here.
    - e.g. `title="More information"`
  - **[PLACE YOUR CONTENT HERE]** - Add the stuff you want displayed in the collapsable box here. You can add other elements outside the `<p>` tags as well such as lists and images, as long as everything stays within the `<div>` tags.
    - If you are not familiar with HTML and you want to add stuff beyond plain text, I'd recommend adding it using the rich text editor at the bottom of the page, then cutting and pasting the source code between the two `<div>` tags.
    - If you need multiple paragraphs, add your additional paragraphs after the closed `</p>` tag enclosed with a `<p>` tag at the beginning and a `</p>` tag at the end.
  



# Formatting Tricks
