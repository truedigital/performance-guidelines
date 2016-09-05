# Performance Guidelines
We have a documented set of guidelines for our performance and optimisation output for our web applications. These guidelines, where applied, allow us to get the best experience for users across a multitude of different devices but are specifically measured against mobile and desktop. The guidelines will constantly be updated to adapt to changes in best practice mainly lead by the rules applied by the Google [Page Insights](https://developers.google.com/speed/pagespeed/insights/) tool. Our performance and optimisation guidelines are at the forefront of our thinking when approaching the development of any web application but are still susceptible to influence from the demands of the web application itself.

## General
* Enable gzip
* Scrolling/animation should keep to 60fps

## CSS
* Concatonate and minify styles

## Images
* Use the appropriate image format (jpg for photo, png8 for flat colors, png24 for transparency)
* Optimise images accordingly (bg images can usually be lower quality)
* Limit scaling of images with CSS
* Use responsive images when able to
* Sprite common SVGs and those that need to be CSS editable
* base64 any SVGs included within CSS
* JPGs should be progressive, for perceived performance
* Consider lazy-loading images
* Always lazy load carousel images

## JavaScript
* Concatonate and minifiy JS
* Include JS at bottom of page
* Limit use of third party scripts
* Pull in large scripts (ie: validation) programatically

## Video
* Try to load video on demand, rather than on page load

## Fonts
* Customise subsetting to only include characters that are needed. 
* Try to refrain from 3rd party font hosting

## Caching
* All server responses should specify a caching policy that dictates when the client can reuse a previously fetched response. In order to adhere to the Page Insights rulings, caching times for static assets should be up to a year with a minimum of one week. This can be achieved through a multitude of different ways as highlighted in this [google doc](https://developers.google.com/web/fundamentals/performance/optimizing-content-efficiency/http-caching#caching-checklist)
