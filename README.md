# css-only-switch
Just a simple HTML and CSS only solution to any switch component/control!

## How does it work ?
In the background it uses an input element for keeping the state (it's "type" can be either a checkbox or a radio).    
The only visible part is the label element (which is connected to the input element with the "for" attribute) - see the "What to keep an eye out for" section below.    
Then it's just about connecting the input's states (:checked) and the label ... and you got a working switch!

The displayed text is kept in the label's data-(true|false) attributes (and the magic thing here is the attr() use in the CSS).    
And of course, you can use the input as you'd do normally - add "name" attribute (for the use in forms), add checked attribute to it (default state change) etc.

## What to keep an eye out for
The input element must be just before the label element (... as we're using the + operator in the CSS)!    
The input element and the label elements MUST have the same "for" (label) and "id" (input) attributes.    
