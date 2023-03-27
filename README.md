# Using tables
Using separate tables will help screen readers understand the document flow.

A particular element to be hidden from screen readers, you need to use the aria-hidden attribute and set it to true
    aria-hidden="true"


# Elements used

caption

thead
tbody
(The thead and tbody elements are used to indicate which portion of your table is the header, and which portion contains the primary data or content.)

tr      is used to indicate a table row. 
td      indicates a data cell.
th      indicates a header cell.

The CSS clip property is used to define the visible portions of an element. 
The clip-path property determines the shape the clip property should take. Set both the clip-path and -webkit-clip-path properties to the value of inset(50%), forming the clip-path into a rectangle within the element.

overflow: hidden;
white-space: nowrap;
    Prevent text from overflowing.

The calc() function is a CSS function that allows you to calculate a value based on other values. For example, you can use it to calculate the width of the viewport minus the margin of an element:

.example {
  margin: 10px;
  width: calc(100% - 20px);
}

border-collapse property to collapse, which will allow cell borders to collapse into a single border, instead of a border around each cell.

# Now let´s talk bout´ Selectors

    *The element/class/id[class~="xyz"] selector will select only any element/class/id whose class includes xyz. 

        ex:  
            The span[class~="sr-only"] selector will select any span element whose class includes sr-only. 

    *The :first-of-type pseudo-selector is used to target the first element that matches the selector.

    *The :last-of-type pseudo-selector does the exact opposite - it targets the last element that matches the selector.

    *The span[class] syntax will target any span element that has a class attribute set, regardless of the attribute's value.

    *The :not() pseudo-selector is used to target all elements that do not match the selector

            ex:
            in this case, any of your span elements that do not have the sr-only class. This ensures that your earlier rules for the span[class~="sr-only"] selector are not overwritten.

            span:not(.sr-only) {
            font-weight: normal;
            }

    *The [attribute="value"] selector targets any element that has an attribute with a specific value.

            ex: 
                tr[class="total"] selector to target specifically your tr elements with the total class

    *The :nth-of-type() pseudo-selector is used to target specific elements based on their order among siblings of the same type.

            ex: 
                tr.total td:nth-of-type(3) {
                    padding-right: 0.5rem;
                }

    *last-of-type
    *first-of-type



