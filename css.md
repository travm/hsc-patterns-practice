#CSS

##Naming Convention

Our CSS will use hyphen-separation for all class and ID names. Please note that this only applies when you class names extend beyond a single word. It is not a requirement that all styles have a two word minimum.

 

##Code Organization

To improve maintainability and efficiency we will be implementing an object-oriented code structure for our CSS. This will create a consistency and expectation for other team members when viewing your code.

###Imports

If you’re using Sass, all mixins and partials should be included here. They will be included in the toolkit by default. Just remember that any additional partials or mixins that you create must be added!

###Base

Base styles are our “global defaults” that we use throughout to define how our HTML elements look by default. This can be used along side Normalize to overwrite those default or you can use Normalize as your base.

###Layouts

Layouts separate and hold modules together to form pages. They are used to control and measure the widths of our main layout columns. Not to be confused with our optional grid system which is only available when using Sass.

###Modules

Modules are modular elements that make up all of the content that can be reused throughout the design. This will more than likely make up a majority of your design and code. Remember, the key is to make our styles as reusable as possible!

###Modifiers

Modifiers change the look or behavior of an element or module. For example, when a user completes a form and it fails validation we can append a modifier class to change the input to a c class with a red background color.

Organizing your code into these sections with modularity in mind will help establish a consistency when viewing fellow team member’s code. This will allow us to stay DRY (Don’t Repeat Yourself) and efficient.

 

##Code Formatting

Readability is an important factor when considering maintainability and efficiency. There is an endless debate on whether single-line or multi-line code formatting is more readable. However, much of it is up to personal preference. To get the best of both worlds, use a mixture of single-line and multi-line code formatting. Each style should start being in a single-line format until the style grows too large and becomes unwieldy. Once this happens, the style should be broken into a multi-line format. The reason to implement both is to save horizontal space where possible.

##Property Ordering

Having a consistent order to our CSS properties is very important to maintainability. As you write CSS make sure to group your properties by their type. For example: font, box model, positioning, text, etc. We will order each group as follows:

 
1. Font
    1. color
    2. font-family
    3. font-size
    4. line-height
    5. text-align

2. Display/Box Model
    1. width
    2. height
    3. padding
    4. margin
    5. background
    6. border
    7. box-sizing
    8. display
    9. overflow

3. Position
    1. position
    2. top, right, left, bottom
    3. z-index

4. Other
    1. cursor

 

##Pre-processing

Ruby-based pre-processor Sass is our optional pre-processor of choice. Due to it’s similarities to vanilla CSS and JavaScript/C-Based programming languages we will be using the .scss file format instead of .sass. All Sass files must use the .scss format. If you choose to take advantage of Sass then you will have to compile the CSS yourself using the command line or any other third party compiling software.

##Partials/Libraries

To extend our optional functionality, there are a number of great partials you can use to help get you started quickly.

###Normalize (_normalize.scss)

In favor of retaining valuable browser defaults for elements we will be using the Normalize CSS library. This will be replacing our use of Eric Meyer’s CSS Reset.

###Shared Mixins (_mixins.scss)

Since we have ruled out using Compass for now, we will be creating some of our own custom mixins that will replicate much of the functionality found in both Compass and Bourbon.IO. As we figure out new ways to use mixins to improve our development process they will be added to this file. If the file begins to get too large or unwieldy we can consider breaking it out into multiple files.

 

###Grid (_grid.scss)

Now we are making use of an optional grid to help create your layouts. The included grid system is Semantic Grid System. This will allow you to handle al of your grid measurements in your CSS without adding tons of non-semantic classes to your HTML. You can use your own grid system, but we highly suggest that you use Semantic.GS.
