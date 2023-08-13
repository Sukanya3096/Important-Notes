# HTML5 Interview Questions and Answers

<br/>

|Sl.No|  Questions                        |
|----|------------------------------------|
| 01.|[What does markup language mean?](#q-what-does-markup-language-mean)|
| 02.|[What are meta tags?](#q-what-are-meta-tags)|
| 03.|[What are the different ways to add CSS?](#q-what-are-the-different-ways-to-add-css)|
| 04.|[What happens when DOCTYPE is not given?](#q-what-happens-when-doctype-is-not-given)|
| 05.|[What is div?](#q-what-is-div)|
| 06.|[What are semantic tags?](#q-what-are-semantic-tags)|
| 07.|[Element vs Tag vs Attribute](#q-element-vs-tag-vs-attribute)|
| 08.|[What is script tag?](#q-what-is-script-tag)|

<br/>


## Q. ***What does markup language mean?***
- Standard text-encoding system consisting of a set of symbols inserted in a text document to control its structure, formatting, or the relationship between its parts.
- The most widely used markup languages are SGML (Standard Generalized Markup Language), HTML (Hypertext Markup Language), and XML (Extensible Markup Language).

## Q. ***What are meta tags?***
- meta tags live within the head tag of the HTML document.
- The head tag is used for configurating the HTML file.
- meta tags represent metadata. They are essentially used for defining and describing data about data, and are used to add extra information to the data inside the webpage.
- There are many meta tags. Some of them help improve the SEO (Search Engine Optimisation) of website, making sure that the content of the site is relevant to what people are searching for.

```html
<!DOCTYPE html>
<html>
  <head>
        <!--Recommended Meta Tags-->
        <meta charset="utf-8">
        <meta name="language" content="english"> 
        <meta http-equiv="content-type" content="text/html">
        <meta name="author" content="Author Name">
        <meta name="designer" content="Designer Name">
        <meta name="publisher" content="Publisher Name">
        <meta name="no-email-collection" content="name@email.com">
        <meta http-equiv="X-UA-Compatible" content="IE=edge"/>

        <!--Search Engine Optimization Meta Tags-->
        <meta name="description" content="Project Description">
        <meta name="keywords" content="Software Engineer,Product Manager,Project Manager,Data Scientist">
        <meta name="robots" content="index,follow">
        <meta name="revisit-after" content="7 days">
        <meta name="distribution" content="web">
        <meta name="robots" content="noodp">
        
        <!--Optional Meta Tags-->
        <meta name="distribution" content="web">
        <meta name="web_author" content="">
        <meta name="rating" content="">
        <meta name="subject" content="Personal">
        <meta name="title" content=" - Official Website.">
        <meta name="copyright" content="Copyright 2020">
        <meta name="reply-to" content="">
        <meta name="abstract" content="">
        <meta name="city" content="Bangalore">
        <meta name="country" content="INDIA">
        <meta name="distribution" content="">
        <meta name="classification" content="">
        
        <!--http-equiv Tags-->
        <meta http-equiv="Content-Style-Type" content="text/css">
        <meta http-equiv="Content-Script-Type" content="text/javascript">
      
    <title>HTML5 Meta Tags</title>
  </head>
  <body>
       ...
  </body>
</html>
```
<div align="right">
    <b><a href="#">↥ back to top</a></b>
</div>


## Q. ***What are the different ways to add CSS?***
1. Inline CSS
The first way to add CSS into HTML is by using a method called ***inline-styling***. Inline-style means adding CSS rules directly into the HTML elements (tags) with the style attribute.

For example,to change the text color of an element:

```html
<h1 style="color: red">Test Headline</h1>
```
However in daily programming, we don’t want to use inline-styles, because it only targets a single HTML element, instead of targeting multiple, is not easily searched and found in larger projects, and the most important reason is that we can’t keep our CSS code separate from HTML.

2. Internal CSS
The second way for adding CSS to HTML is by using the internal CSS way.
In order to use this way, we need to use an HTML tag called <style> tag (not style attribute) and between the style tags, we can write our CSS selectors & rules:

```html
<style>  
  h1 {  
    color: red;
  }
</style>
<body>  
  <h1>Test Headline</h1>
</body>
```
3. External CSS
Keeping CSS & HTML separated is best practice. In real programming, we need to keep HTML, CSS, and JavaScript in separate files and later import them where necessary. This way improves readability & makes it easier for the maintenance of the code.

To use this way, we need to create separate CSS files with an extension of .css and later link them to HTML.

For example, we can create a CSS file like this one: index.css. Inside index.css, we write our CSS rules:

```html
h1 {  
  color: red;
}
```
Then we can import index.css to HTML with a <link> tag like below:

```html
<head>
   <link rel="stylesheet" type="text/css" href="index.css">
</head>
<body>
 <h1> Test Headline </h1>
</body>
```

## Q. ***What happens when DOCTYPE is not given?***

The web page is rendered in quirks mode. The web browsers engines use quirks mode to support older browsers which does not follow the **W3C specifications**. In quirks mode CSS class and id names are case insensitive. In standards mode they are case sensitive.
<div align="right">
    <b><a href="#">↥ back to top</a></b>
</div>

## Q. ***What is div?***
The HTML division tag, called "div" for short, is a special element that lets us group similar sets of content together on a web page. We can use it as a generic container for associating similar content.

## Q. ***What are semantic tags?***
- Semantic HTML elements are those that clearly describe their meaning in a human- and machine-readable way.
- The semantic elements added in HTML5 are:
  ```html
  <article>
  <aside>
  <details>
  <figcaption>
  <figure>
  <footer>
  <header>
  <main>
  <mark>
  <nav>
  <section>
  <summary>
  <time>
  ```
Elements such as
```html
<header> <nav> <section> <article> <aside> and <footer>
```
 act more or less like 
 ```html
 <div> elements.
```
They group other elements together into page sections. However where a div tag could contain any type of information, it is easy to identify what sort of information would go in a semantic header region.

***Why use semantic elements?***
- It is much easier to read.
- It has greater accessibility. You are not the only one that finds semantic elements easier to understand. Search engines and assistive technologies (like screen readers for users with a sight impairment) are also able to better understand the context and content of your website, meaning a better experience for your users.

## Q. ***Element vs Tag vs Attribute***
An element is a single ‘chunk’ of code comprising of an opening and closing tag.

```html
<code><div>This is a div element</div></code>
```
This is a div element. Not a div tag.

Some elements have only one, self-closing tag:
```html
<code><img /></code>
```

Tags are the bits that make up elements. <div> is a tag. An opening and closing tag makes an element:
```html
<code><div></code>
```
And:
```html
<code></div></code>
```
Attributes
An attribute is a piece of code attached to a tag which supplies additional information:
```html
<code><div <mark>class="some-class"</mark>>This is a div element</div></code>
```
This is an attribute.

## Q. ***What is script tag?***
The ```<script>``` tag is known for embedding the scripts like JavaScript. The ```<script>``` tag comes with its attributes which decide behaviour of the tag. One of the example of ```<script>``` attribute is src attribute which provides the path to the external script files.

```html
<script>  
  //code to be executed  
</script>
```









