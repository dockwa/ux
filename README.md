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
* [Spacing](#spacing)
  * [Margin / Padding](#margin--padding)
  * [Whitespace](#whitespace)
* [Hamburger menus](#hamburger-menus)
* [System paradigms](#system-paradigms)
* [User Decisions](#user-decisions)
* [Errors & Loading](#errors--loading)

## Typography

### Uppercasing

Sentence case is always the way to go.
We are taught to read in sentences.
When we read words, we look more at the shapes of the words than each individual letter.
That being said, USING ALL UPPERCASE CAN MAKE THINGS REALLY HARD FOR A USER TO READ.
**There is no place in UI for uppercase text**, it can be "pretty" in design, but the user's experience is greatly degraded by how difficult ALLCAPS is to read.

If you are making an logo, uppercase can be acceptable because you are making an image / icon - not text meant for reading.
Anything that is meant to be read should never use uppercase text. More Info: [Wikipedia article about ALLCAPS](https://en.wikipedia.org/wiki/All_caps), [Succinct UX Explanation](http://uxmovement.com/content/all-caps-hard-for-users-to-read/), [Typographical Explanation](http://practicaltypography.com/all-caps.html), [explanation of how people read](http://www.graphics.com/article-old/how-people-read)

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


## Spacing

### Margin / Padding

Make all margins / padding **equal** around every element on the screen. **Equal margin / padding** will help make the interface more cohesive, look 'more professional', and make elements _fit_ together. **Equal spacing** helps the eyes navigate the content. 

### Whitespace
If you aren't sure if you have enough whitespace, you need more whitespace. Leave plenty of space between elements. Let the eyes breathe. White pixels are free. [More on whitespace here](http://uxmyths.com/post/2059998441/myth-28-white-space-is-wasted-space)

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


## User Decisions

Help the user succeed by not forcing them to make decisions. Aim for **one button / call to action per page**, or otherwise try keep the number of user actions on a page as low as possible. Never make the user ask themself "what do I do now?" **give a clear course of action for every screen** they see.  

## Errors & Loading 

The most important part of any relationship is communication. In the relationship of the user and the app, the app needs to clearly communicate what its doing and when things go wrong. When an error is encountered (such as a network error, an input error, a data validation issue, etc) explain it clearly to the user and give **a single clear course of action** to correct or handle the error. When the app is loading data over the network, **show a loading indicator** so the user knows why the app just stopped responding. Even better, add a line of descriptive text to explain what is loading along with a loading indicator. Clear communication from the app to the user promotes trust between the user and the app. 

