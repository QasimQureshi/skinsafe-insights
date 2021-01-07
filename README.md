# SkinSAFE insights

Testing SkinSAFE insights product badge integration on CVS pharmacy

### How to use insights

Include Insights.js
```
<script data-skinsafe="ssinsight" src="https://her-skinsafe-production.s3-us-west-2.amazonaws.com/insights/insights.js"></script>
```

And then call the **skinSAFEinsights.renderBadges(element, ID, ID-type)** method. The element the DOM element we render badges in. Supported ID types are slugs (like *mario-badescu-drying-lotion-1-fl-oz*), UPC codes ("upc") and product names ("name").
```
document.addEventListener('DOMContentLoaded', function(){
    skinSAFEinsights.renderBadges(
        document.querySelector('.skinsafe-badges'),
        "mario-badescu-drying-lotion-1-fl-oz",
        "slug");
})
```

