Gradient Mixins
-
###{LESS} mixins for linear and radial gradients

A simplified way to create complex multi-colored CSS3 gradients

#### How to use it:
1. Download gradient-mixins.less
2. Import downloaded file `@import "gradient-mixins.less"`.

### Examples:
**{less}:**  
```css
    .element {
        .gradient(0, #FF0000);
    }
```  
**CSS result:**  
```css
    .element {
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
        .gradient-with-hover(0, #FF0000);
    }
```  
**CSS result:**  
```css
    .element {
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



[**@nick11703**](https://github.com/nick11703/)
