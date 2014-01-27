Gradient Mixins
-
###{LESS} mixins for linear and radial gradients

A simplified way to create complex multi-colored CSS3 gradients

#### How to use it:
1. Download gradient-mixins.less
2. Import downloaded file `@import "gradient-mixins.less"`.

```css
@direction = 0-360 for linear or radial for radial
@middleColor = color to be lightened and darkened by 5%
`.gradient(@direction, @middleColor);`
`.gradient-with-hover(@direction, @middleColor));`

@direction = 0-360 for linear or radial for radial
@startColor = color to start the gradient
@endColor = color to end the gradient
`.gradient(@direction, @startColor, @endColor);`
`.gradient-with-hover(@direction, @startColor, @endColor));`
```

### Examples:
**{less}:**  
```css
    .element {
        /* Linear gradient at 0 degrees */
        .gradient(0, #FF0000);
    }
```  
**CSS result:**  
```css
    .element {
        /* Linear gradient at 0 degrees */
        background-color: #ff1a1a;
        background-image: -webkit-gradient(linear, 0% 0%, 0% 100%, from(#ff1a1a), to(#e60000));
        background-image: -webkit-linear-gradient(0deg, #ff1a1a, #e60000);
        background-image: -moz-linear-gradient(0deg, top, #ff1a1a, #e60000);
        background-image: -ms-linear-gradient(0deg, #ff1a1a, #e60000);
        background-image: -o-linear-gradient(0deg, #ff1a1a, #e60000);
        background-image: linear-gradient(0deg, #ff1a1a, #e60000);
        filter: progid:DXImageTransform.Microsoft.gradient(startColorStr='#ff1a1a', EndColorStr='#e60000');
        -ms-filter: "progid:DXImageTransform.Microsoft.gradient(startColorstr=#ffff1a1a, endColorstr=#ffe60000)";
    }
```


**{less}:**  
```css
    .element {
        /* Linear gradient at 0 degrees with hover */
        .gradient-with-hover(0, #FF0000);
    }
```  
**CSS result:**  
```css
    .element {
        /* Linear gradient at 0 degrees with hover */
        background-color: #ff1a1a;
        background-image: -webkit-gradient(linear, 0% 0%, 0% 100%, from(#ff1a1a), to(#e60000));
        background-image: -webkit-linear-gradient(0deg, #ff1a1a, #e60000);
        background-image: -moz-linear-gradient(0deg, top, #ff1a1a, #e60000);
        background-image: -ms-linear-gradient(0deg, #ff1a1a, #e60000);
        background-image: -o-linear-gradient(0deg, #ff1a1a, #e60000);
        background-image: linear-gradient(0deg, #ff1a1a, #e60000);
        filter: progid:DXImageTransform.Microsoft.gradient(startColorStr='#ff1a1a', EndColorStr='#e60000');
        -ms-filter: "progid:DXImageTransform.Microsoft.gradient(startColorstr=#ffff1a1a, endColorstr=#ffe60000)";
    }
    .element:active,
    .element:hover {
        background-color: #e60000;
        background-image: -webkit-gradient(linear, 0% 0%, 0% 100%, from(#e60000), to(#ff1a1a));
        background-image: -webkit-linear-gradient(0deg, #e60000, #ff1a1a);
        background-image: -moz-linear-gradient(0deg, top, #e60000, #ff1a1a);
        background-image: -ms-linear-gradient(0deg, #e60000, #ff1a1a);
        background-image: -o-linear-gradient(0deg, #e60000, #ff1a1a);
        background-image: linear-gradient(0deg, #e60000, #ff1a1a);
        filter: progid:DXImageTransform.Microsoft.gradient(startColorStr='#e60000', EndColorStr='#ff1a1a');
        -ms-filter: "progid:DXImageTransform.Microsoft.gradient(startColorstr=#ffe60000, endColorstr=#ffff1a1a)";
    }
    .element:visited {
        background-color: #ff1a1a;
        background-image: -webkit-gradient(linear, 0% 0%, 0% 100%, from(#ff1a1a), to(#e60000));
        background-image: -webkit-linear-gradient(0deg, #ff1a1a, #e60000);
        background-image: -moz-linear-gradient(0deg, top, #ff1a1a, #e60000);
        background-image: -ms-linear-gradient(0deg, #ff1a1a, #e60000);
        background-image: -o-linear-gradient(0deg, #ff1a1a, #e60000);
        background-image: linear-gradient(0deg, #ff1a1a, #e60000);
        filter: progid:DXImageTransform.Microsoft.gradient(startColorStr='#ff1a1a', EndColorStr='#e60000');
        -ms-filter: "progid:DXImageTransform.Microsoft.gradient(startColorstr=#ffff1a1a, endColorstr=#ffe60000)";
    }
```
**{less}:**  
```css
    .element {
        /* Radial gradient */
        .gradient(radial, #FF0000);
    }
```  
**CSS result:**  
```css
    .element {
        /* Radial gradient */
        background-color: #ff1a1a;
        background-image: -moz-radial-gradient(center, ellipse cover, #ff1a1a, #e60000);
        background-image: -webkit-gradient(radial, center center, 0px, center center, 100%, color-stop(#ff1a1a), color-stop(#e60000));
        background-image: -webkit-radial-gradient(center, ellipse cover, #ff1a1a, #e60000);
        background-image: -o-radial-gradient(center, ellipse cover, #ff1a1a, #e60000);
        background-image: -ms-radial-gradient(center, ellipse cover, #ff1a1a, #e60000);
        background-image: radial-gradient(ellipse at center, #ff1a1a, #e60000);
        filter: progid:DXImageTransform.Microsoft.gradient(startColorStr='#ff1a1a', EndColorStr='#e60000');
        -ms-filter: "progid:DXImageTransform.Microsoft.gradient(startColorstr=#ffff1a1a, endColorstr=#ffe60000)";
    }
```


**{less}:**  
```css
    .element {
        /* Radial gradient with hover */
        .gradient-with-hover(radial, #FF0000, #333333);
    }
```  
**CSS result:**  
```css
    .element {
        /* Radial gradient with hover */
        background-color: #ff0000;
        background-image: -moz-radial-gradient(center, ellipse cover, #ff0000, #333333);
        background-image: -webkit-gradient(radial, center center, 0px, center center, 100%, color-stop(#ff0000), color-stop(#333333));
        background-image: -webkit-radial-gradient(center, ellipse cover, #ff0000, #333333);
        background-image: -o-radial-gradient(center, ellipse cover, #ff0000, #333333);
        background-image: -ms-radial-gradient(center, ellipse cover, #ff0000, #333333);
        background-image: radial-gradient(ellipse at center, #ff0000, #333333);
        filter: progid:DXImageTransform.Microsoft.gradient(startColorStr='#ff0000', EndColorStr='#333333');
        -ms-filter: "progid:DXImageTransform.Microsoft.gradient(startColorstr=#ffff0000, endColorstr=#ff333333)";
    }
    .element:active,
    .element:hover {
        background-color: #333333;
        background-image: -moz-radial-gradient(center, ellipse cover, #333333, #ff0000);
        background-image: -webkit-gradient(radial, center center, 0px, center center, 100%, color-stop(#333333), color-stop(#ff0000));
        background-image: -webkit-radial-gradient(center, ellipse cover, #333333, #ff0000);
        background-image: -o-radial-gradient(center, ellipse cover, #333333, #ff0000);
        background-image: -ms-radial-gradient(center, ellipse cover, #333333, #ff0000);
        background-image: radial-gradient(ellipse at center, #333333, #ff0000);
        filter: progid:DXImageTransform.Microsoft.gradient(startColorStr='#333333', EndColorStr='#ff0000');
        -ms-filter: "progid:DXImageTransform.Microsoft.gradient(startColorstr=#ff333333, endColorstr=#ffff0000)";
    }
    .element:visited {
        background-color: #ff0000;
        background-image: -moz-radial-gradient(center, ellipse cover, #ff0000, #333333);
        background-image: -webkit-gradient(radial, center center, 0px, center center, 100%, color-stop(#ff0000), color-stop(#333333));
        background-image: -webkit-radial-gradient(center, ellipse cover, #ff0000, #333333);
        background-image: -o-radial-gradient(center, ellipse cover, #ff0000, #333333);
        background-image: -ms-radial-gradient(center, ellipse cover, #ff0000, #333333);
        background-image: radial-gradient(ellipse at center, #ff0000, #333333);
        filter: progid:DXImageTransform.Microsoft.gradient(startColorStr='#ff0000', EndColorStr='#333333');
        -ms-filter: "progid:DXImageTransform.Microsoft.gradient(startColorstr=#ffff0000, endColorstr=#ff333333)";
    }
```




[**@nick11703**](https://github.com/nick11703/)
