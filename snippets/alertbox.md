## Alert Box
This is a box of text designed to catch the user's attention with bolder text and different coloring. The Exclaimation point icon contains an Aria label that screen readers will read aloud as "Alert." This is designed to draw the user's attention to important notes/safety notices.
![Screenshot of an alert box. The text is bold and enclosed in a red box with an icon to indicate that the text is important](documentationImages/alertbox.png)
1. Copy and paste the following code wherever your want your alert box to be. It is recommended not to place it inside any inline elements (mostly text elements like `<p>` and such).
```
<div class="alertBox">
   <p>
      <span class="glyphicon glyphicon-exclamation-sign" aria-label="Alert"></span>
      [YOUR MESSAGE HERE]
   </p>
</div>
```
