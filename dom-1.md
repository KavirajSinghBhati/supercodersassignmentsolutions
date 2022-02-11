# DOM Tree: Finding HTML Elements 

![image](https://user-images.githubusercontent.com/59439509/153598633-5f967ded-01de-4132-91ad-b98b44060053.png)
![image](https://user-images.githubusercontent.com/59439509/153598656-5b894dce-2dd5-4104-9c1f-e4d0e3c2cddf.png)

## Task 1: 
Create a function named getSpanWithId, which finds the span element with id 'span-1' and return it.

## Task 2: 
Create a function named getAllSpanTags, which finds all the span elements return them.

## Task 3: 
Create a function named getSpanWithClass, which finds all the span elements with class-name 'red' and return them.

## Task 4: 
Create a function named getMyForm, which finds the form element with id 'my-form' and return it.

``` html

<span id="span-1">this is span 1.</span>
<span>this is span 2.</span>
<span>this is span 3.</span>
<span class="red">this is span 4.</span>
<span class="red">this is span 5.</span>

<form id="my-form">
	<fieldset>
    	<label>username</label>
    	<input name="username" id="username"/>
    </fieldset>
</form>
```

```javascript
function getSpanWithId() {
  let span = document.getElementById("span-1");
  return span;
}

function getAllSpanTags() {
  let allSpans = document.querySelectorAll("span");
  return allSpans;
}

function getSpanWithClass() {
  let redSpans = document.querySelectorAll("span.red");
  return redSpans;
}

function getMyForm() {
  let myForm = document.forms["my-form"];
  return myForm;
}
```
