# Module 01 Challenge
Topic assessed: HTML, CSS, and Git

## My Task

On-the-job ticket&mdash; **Refactoring** existing code/site to make it more accessible.

> Accessible sites rank higher in search engines. 
> Increased assessibility helps companies avoid litigation.

Adhere to the **Scout Rule**&mdash; always leave the code a little cleaner than when you found it.

> Exceed expectations and improve the codebase for long-term sustainability. 
> Check that all links are functioning correctly.
> Increase the efficiency of the CSS by consolidating the selectors and properties.
> Organize CSS to follow the semantic structure of the HTML elements.
> Include comments before each element or section of the page.

## User Story

```
AS A marketing agency
I WANT a codebase that follows accessibility standards
SO THAT our own site is optimized for search engines
```

## Acceptance Criteria

```
GIVEN a webpage meets accessibility standards
WHEN I view the source code
THEN I find semantic HTML elements
WHEN I view the structure of the HTML elements
THEN I find that the elements follow a logical structure independent of styling and positioning
WHEN I view the icon and image elements
THEN I find accessible alt attributes
WHEN I view the heading attributes
THEN they fall in sequential order
WHEN I view the title element
THEN I find a concise, descriptive title
```

## Detailed Updates

* **HTML Updates**: 
  * **Title**: Added concise, descriptive title to <head> element.
  * **Semantic Elements**: Renamed undescriptive <div> elements to descriptive semantic elements.
    * Such as: <header>, <nav>, <figure>, <main>, <section>, <aside>, and <footer>.
  * **Attributes**: Added descriptive alt attributes to images to increase assessibility.
  * **Hero Title**: Added title to hero image for supplemental information tooltip.
  * **Classes**: Consolidated classes of the same style.
    * Consolidated classes "search-engine-optimization", "online-reputation-management", and "social-media-marketing" to class "content".
    * Consolidated classes "benefit-lead", "benefit-brand", and "benefit-cost" to class "benefit".
  * **Links**: Fixed any links that were unfunctional.
    * The link for "search-engine-optimization" in the navigation bar did not have a linked id in the corresponding section.
  * **Heading Attributes**: Changed heading attribute in the footer from <h3> to <h4> to follow sequential order.
  * **Comments**: Added descriptive comments before each element/section on the page.

* **CSS Updates**: 
  * **Order**: Ordered selectors based on the order appeared on HTML.
  * **Element Selectors**: Changed applicable class selectors to element selectors.
    * Certain selectors do not need to be a class, such as: header, nav, h1, h2, and footer element selectors.
  * **Descendant Selectors**: Renamed undescriptive descendant selectors, such as "div", to descriptive element selectors.
    * Changed descendant selector ".header div" to element selector "nav".
  * **Unique Selectors**: Remove unnecesary element selectors and identify unique id selectors.
    * Unique selectors do not need to be descendant selectors.
    * Unique selectors can be id selectors instead of class selectors.
    > Such as ".header h1" and ".header h1 .seo" can just be "h1" and "#seo" respectively.
  * **Properties**: Combine properties into applicable selectors.
    * Such as, properties under the "ul" and "ul li" selectors can be combined without affecting the page output.
  * **Duplicate Selectors**: Consolidated selectors of the same style.
    * Consolidated selectors ".search-engine-optimization", ".online-reputation-management", and ".social-media-marketing" to ".content".
    * Consolidated descendant selectors ".search-engine-optimization h2", ".online-reputation-management h2", and ".social-media-marketing h2" to element selector "h2".
    * Consolidated descendant selectors ".search-engine-optimization img", ".online-reputation-management img", and ".social-media-marketing img" to descendant selector ".content img".
    * Consolidated selectors ".benefit-lead", ".benefit-brand", and ".benefit-cost" to ".benefit".
    * Consolidated descendant selectors ".benefit-lead h3", ".benefit-brand h3", and ".benefit-cost h3" to element selector "h3".
    * Consolidated descendant selectors ".benefit-lead img", ".benefit-brand img", and ".benefit-cost img" to descendant selector ".benefit img".
  * **Comments**: Added indicative comments before selectors.