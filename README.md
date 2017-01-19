# UX

A lot of the concepts may seem simple.
But many of them are easy traps to fall into.
Most of them are concepts that may _look nice_ on screen but have usibility issues.
An interface should almost always weigh usability over looks.

## Contents
* [Typography](#typography)
  * [Uppercasing](#uppercasing)
  * [Line height](#line-height)
  * [Font weight](#font-weight)
  * [Typeface](#typeface)
* [Placeholders](#placeholders)
* [Spacing (margin / padding)](#spacing-margin--padding)
* [Hamburger menus](#hamburger-menus)
* [System paradigms](#system-paradigms)

## Typography

### Uppercasing

Sentence case is always the way to go.
We are taught to read in sentences.
When we read words, we look more at the shapes of the words than each individual letter.
That being said, USING ALL UPPERCASE CAN MAKE THINGS REALLY HARD FOR A USER TO READ.
There is no place in UI for uppercase text, it can be "pretty" in design, but the experience is hurt greatly by how difficult it becomes to read.

If you are making an logo, uppercase can be ok, because you are making and image / icon.
Anything that is meant to be read should never use uppercase text.

### Line height

Allow the eyes room to breath.
Make sure you apply enough line height that text isn't squished.
150% of the font size is a good place to start, giving 50% of the fonts height between two lines.
[More on line height](https://www.quora.com/What-is-the-ideal-line-height-for-readability).

### Font weight

Don't use a font that is too thin.
It can look nice to use a thin font, but remember the text has to be read with human eyes.
No matter how pretty the thinnest font it, consider giving something with a little more weight to be more readible.

### Typeface

Consider using the font native to the device itself.
iPhone app? Use the default San Francisco font - even better, support [Dynamic Type](http://useyourloaf.com/blog/supporting-dynamic-type/) when possible so your app respects the user's preferences.
Android app? Use the default Roboto font.
On the web? Use system fonts.
A custom font can be a cool look for logos and other branding, but giving the user a font they are accustomed to improves readibility. People came to your app or site to _use_ it, not to admire how pretty it is.

## Placeholders

Most of the time a label is more appropriate.
The biggest issues with placeholders is that they dissapear when you start typing.
A label is clear and doesn't dissapear when you type.
Using a placeholder as an example can also lead to confusion by the user whether something is already entered.
[More on placeholders](https://uxdesign.cc/alternatives-to-placeholder-text-13f430abc56f#.36p3oc4qo).

| Bad usage of placeholders | Context disappears when form is completed |
| --- | --- |
| ![Bad example](/img/placeholder-1.png) | ![Bad example](/img/placeholder-2.png) |

## Spacing (margin / padding)

Make all spacing **even** around every element on the screen. **Even spacing** will help make the interface more cohesive, look 'more professional', and make elements _fit_ together. **Even spacing** helps the eyes navigate the content. 

## Hamburger menus

Hamburger menus can be unavoidable, but should be avoided unless absolutely necessary.
Hamburger menus are where features / actions in an interface go to die.
On a mobile app? Use a tab bar instead.
[More on hamburger menus](https://lmjabreu.com/post/why-and-how-to-avoid-hamburger-menus/).
[Funny tweet](https://twitter.com/lukew/status/443425041795928064?ref_src=twsrc%5Etfw).

## System paradigms

Use the native paradigms of the device or operating system.
If you are building for Android, follow [Material Design](https://material.io/guidelines/)
If you are building for iOS, follow Apple's [Human Interface Guidelines](https://developer.apple.com/ios/human-interface-guidelines/overview/design-principles/)
If you are building for the web use native web patterns. For example, use a <select> input isntead of using a custom select dropdown. The <select> will be interpreted by the device you are on and displayed to the user appropriately. 
**Keep the user comfortable with what they know and use every day.**
