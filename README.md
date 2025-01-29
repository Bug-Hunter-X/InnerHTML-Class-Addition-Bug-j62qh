# Uncommon HTML Bug: innerHTML Class Addition
This repository demonstrates a subtle bug related to using innerHTML in HTML to add classes to elements.  The issue arises when attempting to add a class to a newly created element within the innerHTML string.  Directly setting innerHTML completely replaces the existing content, meaning class attributes are lost.

## Bug Description
The bug occurs because `innerHTML` replaces the entire contents of an element. Any attempt to set attributes or classes within the newly created element won't be applied after the `innerHTML` assignment.

## Solution
The solution avoids the `innerHTML` and uses more robust methods of adding elements and classes to the DOM.  This ensures that elements are created and modified correctly without losing class attributes.
