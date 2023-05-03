/* Apply to 1 property */
/* property name | duration */
transition: margin-right 4s;

/* property name | duration | delay */
transition: margin-right 4s 1s;

/* property name | duration | easing function */
transition: margin-right 4s ease-in-out;

/* property name | duration | easing function | delay */
transition: margin-right 4s ease-in-out 1s;

/* Apply to 2 properties */
transition: margin-right 4s, color 1s;

/* Apply to all changed properties */
transition: all 0.5s ease-out;

/* Global values */
transition: inherit;
transition: initial;
transition: revert;
transition: revert-layer;
transition: unset;
The transition property is specified as one or more single-property transitions, separated by commas.

Each single-property transition describes the transition that should be applied to a single property (or the special values all and none). It includes:

zero or one value representing the property to which the transition should apply. This may be any one of:
the keyword none
the keyword all
a <custom-ident> naming a CSS property.
zero or one <easing-function> value representing the easing function to use
zero, one, or two <time> values. The first value that can be parsed as a time is assigned to the transition-duration, and the second value that can be parsed as a time is assigned to transition-delay.
See how things are handled when lists of property values aren't the same length. In short, extra transition descriptions beyond the number of properties actually being animated are ignored.

Formal definition
Initial value	as each of the properties of the shorthand:
transition-delay: 0s
transition-duration: 0s
transition-property: all
transition-timing-function: ease
Applies to	all elements, ::before and ::after pseudo-elements
Inherited	no
Computed value	as each of the properties of the shorthand:
transition-delay: as specified
transition-duration: as specified
transition-property: as specified
transition-timing-function: as specified
Animation type	discrete
Formal syntax
transition = 
  <single-transition>#  

<single-transition> = 
  [ none | <single-transition-property> ]  ||
  <time>                                   ||
  <easing-function>                        ||
  <time>                                   

<single-transition-property> = 
  all             |
  <custom-ident>  

<easing-function> = 
  linear                          |
  <linear-easing-function>        |
  <cubic-bezier-easing-function>  |
  <step-easing-function>          

<linear-easing-function> = 
  linear( <linear-stop-list> )  

<cubic-bezier-easing-function> = 
  ease                                                |
  ease-in                                             |
  ease-out                                            |
  ease-in-out                                         |
  cubic-bezier( <number [0,1]> , <number> , <number [0,1]> , <number> )  

<step-easing-function> = 
  step-start                                |
  step-end                                  |
  steps( <integer> [, <step-position> ]? )  

<linear-stop-list> = 
  [ <linear-stop> ]#  

<step-position> = 
  jump-start  |
  jump-end    |
  jump-none   |
  jump-both   |
  start       |
  end         

<linear-stop> = 
  <number>               &&
  <linear-stop-length>?  

<linear-stop-length> = 
  <percentage>{1,2}  

Examples
Simple example
This example performs a four-second font size transition with a one-second delay when the user hovers over the element.

HTML
<a class="target">Hover over me</a>
Copy to Clipboard
CSS
.target {
  font-size: 14px;
  transition: font-size 4s 1s;
}

.target:hover {
  font-size: 36px;
}
