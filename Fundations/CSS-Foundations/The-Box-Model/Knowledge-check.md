# Topic: Knowledge check

# Link: https://www.theodinproject.com/lessons/foundations-the-box-model#knowledge-check

1. From inside to outside, what is the order of box-model properties?

- Content-box
- Padding-box
- Border-box
- Margin-box


2. What does the box-sizing CSS property do?

If box-sizing property with value border-box
it change the way standard css box model work, working in an alternative way that takes the border and padding and subtract from the content box, so to respect the with and height declared in the css.

In the standard box model, border and padding will be add to the total size, creating problems in the layout.


3. What is the difference between the standard and alternative box model?
Standard box model will add padding and border to the total width and height, and alternative box model (box-sizing: border-box) will subtract the padding and border from the content box respecting the width and heigh set, this way won't increase size and break layouts.

4. Would you use margin or padding to create more space between 2 elements?
Would use margin, since is the right property to use in this case. padding will only add a white space between the border and the content.

5. Would you use margin or padding to create more space between the contents of an element and its border?
Would use padding, since is the correct property in this case, margin is used to separate elements boxes.

6. Would you use margin or padding if you wanted two elements to overlap each other?
Would use margin, as padding don't accept negative numbers.



7. How do you set the alternative box model for all of your elements?

using the universal element *. In firefox MSN they added something new. The use of the pseudo element ::before and ::after with the box-sizing: border-box;

8. How do you center an element horizontally?
it only work horizontally:
margin: 0 auto;
This means top and bottom 0 and left-right auto. This will effectively center an element in the page, but wont work vertically.