1. Start with the following base code:
```
<div class="flexcontainer">
  <div class="flexbox"><img alt="[ALT TEXT FOR IMAGE OF MACHINE]" loading="lazy" src="[LINK TO MACHINE IMAGE]" /></div>

  <div class="flexbox">
    <h3>[MACHINE NAME]</h3>
    <p><span class="accented">Machine Type:</span> [TYPE OF MACHINE]</p>
    <p><span class="accented">Training Required:</span> [TRAINING REQUIRED]</p>
    <p class="accented">Features and Specs:</p>
    <ul>
      <li>[FEATURE 1]</li>
      <li>[FEATURE 2]</li>
      <li>[AND SO ON...]</li>
    </ul>
    <p><span class="accented">Cost: </span><a href="https://library.charlotte.edu/technology-equipment/area-49/makerspace#fees">View pricing</a></p>
</div>
</div>
```
2. Replace the following placeholders:

   - `[ALT TEXT FOR IMAGE OF MACHINE]` - alt text for the image of the machine
   - `[LINK TO MACHINE IMAGE]` - URL that leads to the image of the machine
   - `[MACHINE NAME]` - the machine's name
   - `[TYPE OF MACHINE]` - What type of machine is it? 3D printer, laser cutter, etc.
   - `[TRAINING REQUIRED]` - Does it require training? If no, put "No" and if yes, then put
       - `<a href="[https://instructure.charlotte.edu/enroll/7JBFKG](https://library.charlotte.edu/technology-equipment/technology-instruction)">Yes, enroll now!</a>`
   - `[FEATURE 1, 2, ETC.]` - List the features of the machine, such as the build volume. Put each list item between `<li>` and `</li>`. You can add more if you want.
