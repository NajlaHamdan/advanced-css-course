# grid property for container
-- justifi-items
-- align-items
Aligns flex items along the cross axis of the current line of the flex container.
-- justify-content
-- align-content
grid property for items


# feature queries

Feature queries are created using the CSS at-rule @supports, and are useful as they give web developers a way to test to see if a browser has support for a certain feature, and then provide CSS that will only run based on the result of that test. In this guide you will learn how to implement progressive enhancement using feature queries.

@supports (display:grid){
    display:grid;
    grid-template-rows:repeat(3,1fr);
}