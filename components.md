# EJS Partials
The main concept of **Partials** is to put a bunch of codes into files that you are going to use them later in multiple pages.

***For example, let say we usually see two contents that used in every single web page that you build, which they are a navbar and footer. So imagine you create inside the 'views' folder a 'partials' folder which includes navbar and footer.***

Lets take a look on these codes.
- navbar.ejs
```
<div class="header clearfix">
        <nav>
            <ul class="nav">
                <li role="presentation"><a href="/">Home</a></li>
            </ul>
            <h3 class="projects">Projects List</h3>
        </nav>
    </div>
```

- footer.ejs
```
<footer class="footer">
        <p>© 2020 Engineering Stuff.</p>
    </footer>
```

Then, we go straightforward to any page to type an include syntax for both (navbar and footer), for example:

```
<%- include('partials/navbar') %>
```
***Don't forget to do not include the file path.***

The reference of this markdown was this [link](https://medium.com/@henslejoseph/ejs-partials-f6f102cb7433).