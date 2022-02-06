# Assignment - Book Review Blog

## Task 1
Create 6 <div> elements with ids 'author', 'post-1', 'post-2', 'post-3', 'related-content' and 'contact-details'.

## Task 2
Add an <img> element child to each <div> with ids 'author', 'post-1', 'post-2', 'post-3'. 'src' attribute must be as per the data below:

Note: Image 'src' is given corresponding to the id of div container.

- author: https://www.bsn.eu/wp-content/uploads/2016/12/user-icon-image-placeholder.jpg

- post-1: https://cdn.lifehack.org/wp-content/uploads/2015/03/tumblr_nd4wnpO3ZS1tv8vcro1_r1_1280.jpg

- post-2: https://cdn.lifehack.org/wp-content/uploads/2015/03/Hobbit_book.jpg

- post-3: https://cdn.lifehack.org/wp-content/uploads/2015/03/71h2sjik5al-_sl1380_.jpg

## Task 3
Add an <h3> element with text 'by John Doe | 1 day ago' inside the div with id 'author'.

## Task 4
Add <h2> elements with text corresponding to the container div ids from below data inside div with ids 'post-1', 'post-2', 'post-3'.

Note: h2 text is given corresponding to the id of div container.

- post-1: Fahrenheit 451, by Ray Bradbury

- post-2: The Hobbit, by J.R.R. Tolkien

- post-3: The Book Thief, by Markus Zusak

## Task 5
Add paragraphs to your posts by adding <p> elements with a text of minimum 50 words inside div with ids 'post-1', 'post-2', 'post-3'.

## Task 6
Set width and height attribute of every <img> element to 300.

## Task 7
Add an <h4> element with text 'Related Content' inside the div with id 'related-content'.

## Task 8
Add a <ul> element with four <li> children containing relevant text inside the div with id 'related-content'.

## Task 9
Add a <p> element with text 'email: john.doe@example.com | phone: +91-12345-67890' inside the div with id 'contact-details'.

## Task 10
Encapsulate 'email:' and 'phone:' texts inside the paragraph of div with id 'contact-details' using <strong> element to make it appear bolder.
  
  
```html
  
<!-- Insert HTML Body Content Here! -->

<style>
  img {
    width: 300px;
    height: 300px;
  }
</style>

<div id = "author">
  <img src="https://www.bsn.eu/wp-content/uploads/2016/12/user-icon-image-placeholder.jpg" />
  <h3>by John Doe | 1 day ago</h3>
</div>
<div id = "post-1">
  <img src="https://cdn.lifehack.org/wp-content/uploads/2015/03/tumblr_nd4wnpO3ZS1tv8vcro1_r1_1280.jpg" />
  <h2>Fahrenheit 451, by Ray Bradbury</h2>
  <p>nulla aliquet porttitor lacus luctus 
    accumsan tortor posuere ac ut consequat 
    semper viverra nam libero justo laoreet 
    sit amet cursus sit amet dictum sit amet 
    justo donec enim diam vulputate ut 
    pharetra sit amet aliquam id diam maecenas 
    ultricies mi eget mauris pharetra et ultrices 
    neque ornare aenean euismod elementum</p>
</div>
<div id = "post-2">
  <img src="https://cdn.lifehack.org/wp-content/uploads/2015/03/Hobbit_book.jpg" />
  <h2>The Hobbit, by J.R.R. Tolkien</h2>
  <p>nulla aliquet porttitor lacus luctus 
    accumsan tortor posuere ac ut consequat 
    semper viverra nam libero justo laoreet 
    sit amet cursus sit amet dictum sit amet 
    justo donec enim diam vulputate ut 
    pharetra sit amet aliquam id diam maecenas 
    ultricies mi eget mauris pharetra et ultrices 
    neque ornare aenean euismod elementum</p>
</div>
<div id = "post-3">
  <img src="https://cdn.lifehack.org/wp-content/uploads/2015/03/71h2sjik5al-_sl1380_.jpg" />
  <h2>The Book Thief, by Markus Zusak</h2>
  <p>nulla aliquet porttitor lacus luctus 
    accumsan tortor posuere ac ut consequat 
    semper viverra nam libero justo laoreet 
    sit amet cursus sit amet dictum sit amet 
    justo donec enim diam vulputate ut 
    pharetra sit amet aliquam id diam maecenas 
    ultricies mi eget mauris pharetra et ultrices 
    neque ornare aenean euismod elementum</p>
</div>
<div id = "related-content">
  <h4>Related Content</h4>
  <ul>
    <li>lorem ipsum</li>
    <li>lorem ipsum</li>
    <li>lorem ipsum</li>
    <li>lorem ipsum</li>
  </ul>
</div>
<div id = "contact-details">
  <p><strong>email:</strong> john.doe@example.com | <strong>phone:</strong> +91-12345-67890</p>
</div>
``` 
