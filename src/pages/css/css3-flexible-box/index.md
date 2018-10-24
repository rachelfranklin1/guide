---
title: CSS3 Flexible Box
---
## CSS3 Flexible Box
The Flexbox model provides for an efficient way to layout, align, and distribute space among elements within your document — even when the viewport and the size of your elements is dynamic or unknown. This is extremely useful when developing a site which will be viewed on different screen sizes.

The most important idea behind the Flexbox model is that the parent container can alter its items' width/height/order to best fill the available space. A flex container expands items to fill available free space, or shrinks them to prevent overflow.<sup>1</sup>


<!-- The article goes here, in GitHub-flavored Markdown. Feel free to add YouTube videos, images, and CodePen/JSBin embeds  -->
#### Basic usage
Flexbox can be used to align any amount of given elements inside one element (the parent container). A basic example of this is the following code:

``` css
.parent-container {
  display: flex;
  flex-direction: row;
  justify-content: center;
}
```

In the example above we: 
- turned the parent element into a flexible container by passing the `display: flex` property.
- we also specified to flexbox how we want it to view the items inside its container using `flex-direction` - the default value is row, but you can pass `column`, `row-reverse`, `column-reverse`. 

Once that's settled, we can start organising our children elements inside the parent container. There are two main ways to do this:

- using `justify-content`; to align your child elements along the main axis of the container. For rows, this is the horizontal line running through the center of the container and for columns, its the vertical line. 
- or by using `align-items:` this will align the child elements along the cross axis. For rows, this will be the vertical line running through the center or for columns, it will be the horizontal line. 

You can see a depiction of the flexbox container with its axis here: 
![flexbox container](https://css-tricks.com/wp-content/uploads/2011/08/flexbox.png)

Values which you can pass to `justify-content:` are:

- `center;`  this will align all of the items along the main axis to the centre of the flex-container.

- `flex-start;` this aligns all of the items to the start of the main axis. This is to the left if the elements are in a row or to the top if they are in a column.

- `flex-end;`  this does the opposite of the above and aligns the items to the end of their main axis (right if row, bottom if column). 

- `space-between;` this will align the first and last item to the beginning and end of the main axis and will evenly distribute the items in between.space-around; space is distributed evenly around all of the items.

Values which can be passed to `align-items` are:

- `flex-start;` items will be aligned to the start of the cross axis. This will be to the top of the container for rows and to the left for columns.

- `flex-end;` items will be aligned to the end of the cross axis. This will be the bottom of the container for rows and to the right for columns. center; there will be equal space outside the items; to the left or right of columns and top or bottoms for rows. 

- `stretch;` items will stretch to fill the container along the cross axis. This means that rows will expand vertically and columns will stretch horizontally. baseline; aligns items to their baselines.


#### More Information:
To get a complete understanding of Flexbox, read <a href="https://medium.freecodecamp.org/understanding-flexbox-everything-you-need-to-know-b4013d4dc9af" target='_blank' rel="nofollow">Understanding Flexbox Everything you need to know</a> on the FreeCodeCamp Medium page.

For an interactive guide go through <a href="https://medium.freecodecamp.org/the-ultimate-guide-to-flexbox-learning-through-examples-8c90248d4676" target="_blank" rel="nofollow">The Ultimate Guide to Flexbox — Learning Through Examples</a>

Both of these are great resources by Ohans Emmanuel. 

Yet another great visual guide that is in-depth but easy to follow can be found in <a href="https://css-tricks.com/snippets/css/a-guide-to-flexbox/" target="_blank" rel="nofolow"> A Guide to Flexbox</a> by <a href="https://css-tricks.com" target="_blank" rel="nofolow">CSS-Tricks</a>

### Sources

1. <a href="https://css-tricks.com/snippets/css/a-guide-to-flexbox/" target="_blank" rel="nofolow">Coyier, Chris. "A Complete Guide to Flexbox" CSS-Tricks. Last updated on September 28, 2017.</a>


