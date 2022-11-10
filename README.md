# Module 01 Challenge- Horiseon Social Solution Services, Inc.

>**Application Link:** [Horiseon Social Solution Services, Inc.](https://fannychen623.github.io/Challenge-01-Horiseon-Social-Solution-Services-Inc/)
>
>**View:** [Description](#description) / [Change Details](#change-details)
>
>**Site Preview:**
>
>![Horiseon Social Solution Services, Inc.](/Assets/01-html-css-git-homework-demo.png "Horiseon Social Solution Services, Inc.")

## **DESCRIPTION**

> Topic Assessed: **HTML**, **CSS**, and **Git**

### **My Task**

*Refactor* existing code/site to make it more accessible.

> Accessible sites rank higher in search engines. 
>
> Increased assessibility helps companies avoid litigation.

Adhere to the *Scout Rule*&mdash; always leave the code a little cleaner than when you found it.

> Exceed expectations and improve the codebase for long-term sustainability. 
>
> Check that all links are functioning correctly.
>
> Increase the efficiency of the CSS by consolidating the selectors and properties.
>
> Organize CSS to follow the semantic structure of the HTML elements.
>
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

## **CHANGE DETAILS**

### HTML Updates
* **Comments**: Added descriptive comments before each element/section on the page.
* **Title**: Added concise, descriptive title to the `<head>` element.
* **Semantic Elements**: Renamed undescriptive `<div>` elements to descriptive semantic elements.
  * Such as: `<header>`, `<nav>`, `<figure>`, `<main>`, `<section>`, `<aside>`, and `<footer>`.
* **Attributes**: Added descriptive *alt* attributes to images to increase assessibility.
* **Hero Title**: Added title to hero image for supplemental information tooltip.
* **Classes**: Consolidated classes of the same style.

    | | | | | Consolidated Class |
    |  :---:  |  :---:  |  :---:  |  :---:  |  :---:  |
    | search-engine-optimization | online-reputation-management | social-media-marketing | &#8594; | **content** |
    | benefit-lead | benefit-brand | benefit-cost | &#8594; | **benefit** |

* **Links**: Fixed any links that were unfunctional.
  * The link for `search-engine-optimization` in the navigation bar did not have a linked id in the corresponding section.
* **Heading Attributes**: Changed heading attribute in the footer from `<h3>` to `<h4>` to follow sequential order.

### CSS Updates
* **Comments**: Added indicative comments before selectors.
* **Order**: Ordered selectors based on the order appeared on HTML.
* **Element Selectors**: Changed applicable class selectors to element selectors.
  * Certain selectors do not need to be a class, such as: `header`, `nav`, `h1`, `h2`, and `footer` element selectors.
* **Descendant Selectors**: Renamed undescriptive descendant selectors, such as `div`, to descriptive element selectors.
  * Changed descendant selector `.header div` to element selector `nav`.
* **Unique Selectors**: Remove unnecesary element selectors and identify unique id selectors.
  * Unique selectors do not need to be descendant selectors.
  * Unique selectors can be id selectors instead of class selectors.
    * Such as `.header h1` and `.header h1 .seo` can just be `h1` and `#seo` respectively.
* **Properties**: Combine properties into applicable selectors.
  * Such as, properties under the `ul` and `ul li` selectors can be combined without affecting the page output.
* **Duplicate Selectors**: Consolidated selectors of the same style.

    | **Class Selectors** | **Descendant Selectors** | **Descendant Selectors**  |
    |  :---:  |  :---:  |  :---:  |
    | .search-engine-optimization | .search-engine-optimization h2 | .search-engine-optimization img |
    | .online-reputation-management | .online-reputation-management h2 | .online-reputation-management img |
    | .social-media-marketing | .social-media-marketing h2 | .social-media-marketing img |
    | &#8595; | &#8595; | &#8595;|
    | **Class Selector** | **Element Selector** | **Descendant Selector** |
    | .content | h2 | .content img |

    | **Class Selectors** | **Descendant Selectors** | **Descendant Selectors**  |
    |  :---:  |  :---:  |  :---:  |
    | .benefit-lead | .benefit-lead h3 | .benefit-lead img |
    | .benefit-brand | .benefit-brand h3 | .benefit-brand img |
    | .benefit-cost | .benefit-cost h3 | .benefit-cost img |
    | &#8595; | &#8595; | &#8595;|
    | **Class Selector** | **Element Selector** | **Descendant Selector** |
    | .benefit | h3 | .benefit img |