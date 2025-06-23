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
- Some elements like images only have a singular tag, which looks like this:
```
<img href="blahblahblah.com/image" alt="Alternate text" />
```
- Notice that instead of a closing tag, this image element has a `/>` at the end.
- This element also has attributes (`href="blahblahblah.com/image"` and `alt="Alternate text"`), which are little bits of text that tell the computer how to display the element. These are usually in the opening tag.
## Details Dropdown
This element will put a question mark icon wherever you paste the code that opens a collapsing box for images/more details/explanations/etc. It looks best when placed at the end of a line. It is classed as a button and styled to look a little better inline.



# Formatting Tricks
