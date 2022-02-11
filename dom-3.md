# DOM Tree: Adding or Deleting Elements 

![image](https://user-images.githubusercontent.com/59439509/153606559-d7cb433b-a25e-482e-b082-420c0a0d8c57.png)
![image](https://user-images.githubusercontent.com/59439509/153606585-71cb6a92-7502-4138-9a04-4fabbddef90a.png)

## Task 1
Create a function named addDivWithSpans, which creates a div element with id 'my-div' containing at least 3 non-empty span elements.

## Task 2
Create a function named removeParagraphs, which finds and removes all the paragraph elements.

```html
<!-- Do not change the below code -->

<p>this is para 1.</p>
<p>this is span 2.</p>
```

```javascript
let div = document.createElement('div');
function addDivWithSpans() {
  div.id = "my-div";
  div.innerHTML = "<span>This is a span</span>";
  div.innerHTML = "<span>This is a span</span>";
  div.innerHTML = "<span>This is a span</span>";
  document.body.appendChild(div);
}

function removeParagraphs() {
  let allP = document.body.querySelectorAll("p");
  allP.forEach(function(item) {
    document.body.removeChild(item);
  });
}
```
