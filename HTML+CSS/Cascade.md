# Cascade

Stylesheets [cascade] the order of CSS rules matters. When two rules apply that have equal specificity, the one that come **LAST** in the CSS is the one that will be used.

## Rules
-   An element selector is less specific — it will select all elements of that type that appear on a page and therefore gets a lower score.
-   A class selector is more specific — it will select only the elements on a page that have a specific `class` attribute value thus will get a higher score.