# DOM Tree: Changing HTML Elements

![image](https://user-images.githubusercontent.com/59439509/153600329-15210a09-a4ce-4ecb-9838-dc67a6938154.png)
![image](https://user-images.githubusercontent.com/59439509/153600528-fb6e012b-14ca-4cf6-8de3-adb0c7f0ef95.png)


## Task 1: 
Create a function named setInnerHTML, which accepts two parameters named element and innerHTML 
respectively, and set the passed innerHTML params to the innerHTML property of the given element.

## Task 2: 
Create a function named setElementAttribute, which accepts three parameters 
named element and attribute, value respectively, and set the passed attribute property to the value parameter.

## Task 3: 
Create a function named setElementStyle, which accepts three parameters named 
element and styleName, value respectively, and set the passed style name property to the value parameter.

```html
<!-- Do not change the below code -->

<p align="center" id="my-paragraph">this is para 1.</p>

<div id="my-div"></div>
```

```javascript
function setInnerHTML(element, innerHTML) {
  element.innerHTML = innerHTML;
}

function setElementAttribute(element, attribute, value) {
  element.setAttribute(attribute, value);
}

function setElementStyle(element, styleName, value) {
  element.style[styleName] = value;
}
```
