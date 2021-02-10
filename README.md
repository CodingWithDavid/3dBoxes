# Create a page using 3d boxes that show an animated gif

This is a simple looking application that will display an animated gif in boxes that go from 3d to plain and back.

by [David Gallivan](http://twitter.com/CodingwithDavid)


## Why

I found this as a java-script project and I thought it would be fun to do in Blazor.  And I was right.

## Getting Started

1. Clone this repository

   ```Command Line
   git clone https://github.com/CodingWithDavid/3dBoxes
   cd 3dBoxes
   ```

1.	Open in Visual Studio or Visual Code
a.	With Visual Code you will need to install the C# extensions
2.	Press F5

## What's in the App

1. Cool button click
   a. It gives the effect of being pushed down and back up
2. Toggling a class on and off via code
   a. This is a common action that needs to be done when a user clicks on something
   b. Add this in the class attribute of the div
   c. `@(goBig ? "big" : "")`
3. In style positioning via code
   a. The background image has to be place differently in each box so that it appears to show the entire image
   b. To achieve this, we call a method to calculate the position within the in-line style
       i. `style='@GetPosition(jj,ii)'`
   c. The method returns a string with the style and values we need
       i. `return $"background-position:{-j * 125}px {-i * 125}px";`
4. CSS animation
   a. As the magic button is clicked, the boxes animate in and out.


## [Demo](https://runbatmanrun.z22.web.core.windows.net/)

## Problems or Suggestions

[Open an issue here]( https://github.com/CodingWithDavid/3dBoxes/issues)

## Thank You


## Resources

- [VS Code](https://code.visualstudio.com)
- [Visual Studio]( https://visualstudio.microsoft.com/)



