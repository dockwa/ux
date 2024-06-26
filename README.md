# UX

A lot of the concepts may seem simple.
But many of them are easy traps to fall into.
Some are designs that may _look nice_ on screen but have usibility issues.
An interface should always value **usability over looks**.
We are designing interfaces to be used, so usability and readability are always more important than how 'pretty' the interface is. That being said, if you follow the guidelines below, you will end up with a clear and simple interface that is both good-looking and very usable. A good explanation of some of the philosophies and techniques described in this guide can be found in this article about ["Complexion Reduction"](https://medium.com/swarm-nyc/complexion-reduction-a-new-trend-in-mobile-design-cef033a0b978#.ly9x7zosu).

## Contents
* [Typography](#typography)
  * [Uppercase](#uppercase)
  * [Line height](#line-height)
  * [Font weight](#font-weight)
  * [Typeface](#typeface)
  * [Alignment](#alignment)
* [Placeholders](#placeholders)
* [Spacing](#spacing)
  * [Margin / Padding](#margin--padding)
  * [Whitespace](#whitespace)
* [Hamburger menus](#hamburger-menus)
* [System paradigms](#system-paradigms)
* [User Decisions](#user-decisions)
* [Errors & Loading](#errors--loading-avoiding-awkward-ui)
* [Touch Interfaces](#touch-interfaces)

## Typography

### Uppercase
_Do **not** use ALLCAPS!_

Sentence case is always the way to go.
We are taught to read in sentences.
When we read words, we look more at the shapes of the words than each individual letter.
That being said, USING ALL UPPERCASE CAN MAKE THINGS REALLY HARD FOR A USER TO READ.
**There is no place in UI for uppercase text**, it can be "pretty" in design, but the user's experience is greatly degraded by how difficult ALLCAPS is to read.

If you are making a logo, uppercase can be acceptable because you are making an image / icon - not text meant for reading.
Anything that is meant to be read should never use uppercase text. More Info: [Wikipedia article about ALLCAPS](https://en.wikipedia.org/wiki/All_caps), [succinct explanation relating to UX](http://uxmovement.com/content/all-caps-hard-for-users-to-read/), [longer form, typographical explanation](http://practicaltypography.com/all-caps.html), [explanation of how people read](http://www.graphics.com/article-old/how-people-read).

### Line height
_Try to keep it at 150% of the font size._

Allow the eyes room to breath.
Make sure you apply enough line height that text isn't squished.
150% of the font size is a good place to start, giving 50% of the fonts height between two lines.
[More on line height](https://www.quora.com/What-is-the-ideal-line-height-for-readability).

### Font weight
_Not too thin / light._

Don't use a font that is too thin.
It can look nice to use a thin font, but remember the text has to be read with human eyes.
No matter how pretty the thinnest font it, consider giving something with a little more weight to be more readible.

### Typeface
_Use the platform's native typeface._

Consider using the font native to the device itself.
iPhone app? Use the default San Francisco font - even better, support [Dynamic Type](http://useyourloaf.com/blog/supporting-dynamic-type/) when possible so your app respects the user's preferences.
Android app? Use the default Roboto font.
On the web? Use system fonts.
A custom font can be a cool look for logos and other branding, but giving the user a font they are accustomed to improves readibility. People came to your app or site to _use_ it, not to admire how pretty it is.

### Alignment
_Don't center align text if it runs longer than one line._

Centered text can be good for buttons, short lines of text, or call outs like headers to add visual symmetry to a page. When text runs longer than one line though it gets hard to read and gets the "Christmas Tree Effect" because it looks like a Christmas tree or text coming out both sides. Prefer to stick to left aligning text for longer more readable text.

| Left aligned | Title and button look ok but paragraph is awkward to read |
| --- | --- |
| ![Left aligned](https://dockwa.github.io/ux/img/alignment-1.png) | ![Center aligned](https://dockwa.github.io/ux/img/alignment-2.png) |

## Placeholders
_Don't use them._

Most of the time a label is more appropriate.
The biggest issues with placeholders is that they dissapear when you start typing.
A label is clear and doesn't dissapear when you type.
Using a placeholder as an example can also lead to confusion by the user whether something is already entered.
[More on placeholders](https://uxdesign.cc/alternatives-to-placeholder-text-13f430abc56f#.36p3oc4qo).

| Bad usage of placeholders | Context disappears when form is completed |
| --- | --- |
| ![Bad example](https://dockwa.github.io/ux/img/placeholder-1.png) | ![Bad example](https://dockwa.github.io/ux/img/placeholder-2.png) |


## Spacing

### Margin / Padding
_Keep it equal._

Make all margins / padding **equal** around every element on the screen. **Equal margin / padding** will help make the interface more cohesive, look 'more professional', and make elements _fit_ together. **Equal spacing** helps the eyes navigate the content.

### Whitespace
_You probably need more._

If you aren't sure if you have enough whitespace, you need more whitespace. Leave plenty of space between elements. Let the eyes breathe. White pixels are free. [More on whitespace here](http://uxmyths.com/post/2059998441/myth-28-white-space-is-wasted-space).

## Hamburger menus
_Avoid at all costs!_

Hamburger menus can be unavoidable, but should be avoided unless absolutely necessary.
Hamburger menus are where features / actions in an interface go to die.
On a mobile app? Use a tab bar instead.
[More on hamburger menus](https://lmjabreu.com/post/why-and-how-to-avoid-hamburger-menus/).
[Funny tweet](https://twitter.com/lukew/status/443425041795928064?ref_src=twsrc%5Etfw).

## System paradigms
_Keep the user comfortable with what they know and use every day._

Use the native paradigms of the device or operating system.
If you are building for Android, follow [Material Design](https://material.io/guidelines/)
If you are building for iOS, follow Apple's [Human Interface Guidelines](https://developer.apple.com/ios/human-interface-guidelines/overview/design-principles/)
If you are building for the web use native web patterns. For example, use a \<select\> input instead of using a custom select dropdown. The \<select\> will be interpreted by the device you are on and displayed to the user appropriately.


## User Decisions
_Aim for one action per screen._

Help the user succeed by not forcing them to make decisions. Aim for **one button / call to action per page**, or otherwise try keep the number of user actions on a page as low as possible. Never make the user ask themself "what do I do now?" **give a clear course of action for every screen** they see.

## Errors & Loading (avoiding 'Awkward UI')
_Clearly communicate app state to the user._

The most important part of any relationship is communication! In the relationship of the user and the app, the app needs to clearly communicate what it's doing and when things go wrong. Clear communication from the app to the user promotes trust with the product, and by extension, trust between the customer and the brand. [Here's a highly recommended article about avoiding 'Awkward UI'.](http://scotthurff.com/posts/why-your-user-interface-is-awkward-youre-ignoring-the-ui-stack)

**Handle all errors:** When an error is encountered (such as a network error, a data validation error, or other unexpected situation, etc) explain to the user what happened in simple, clear, positive, and fun language without getting technical or too wordy (as a general rule, users don't read, so be as concise as possible!) When appropriate, include an error code or HTTP status code to help customer support (and future you!) in reproducing and debugging the issue. Along with telling the user what went wrong, give **a single clear course of action** to correct or handle the error.

**Show app state:** When the app is loading data over the network or performing a long running operation, **show a loading indicator** so the user knows what is going on. Even better, add descriptive and fun copy to explain what is loading along with the loading indicator. 


## Touch Interfaces
_Make all touch targets at least 75x75pts._

When designing interfaces that are intended to (or might be) used on a device with a touch screen (in 2017 that is nearly any website and definitely any native app), make sure that all 'touch targets' are large enough to be comfortably tapped with a finger. An ideal touch target is at least 12mm-15mm, or about 75pts-95pts. [Generous whitespace](#whitespace) with [equal margin / padding](#margin--padding) around all touch targets will also help to make your interface more touchable. [Detailed article on appropriately sizing touch targets here.](http://scotthurff.com/posts/how-to-make-truly-tappable-user-interfaces)

