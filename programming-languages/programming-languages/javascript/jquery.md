# jQuery

### Downloading jQuery

To get started, first download a copy of jQuery and include it in your document. There are two versions of jQuery available for downloading — _compressed_ and _uncompressed_.

The uncompressed file is best suited for development or debugging; while, the minified and compressed file is recommended for production because it saves the precious bandwidth and improves the performance due to small file size.

You can download jQuery from here: [https://jquery.com/download/](https://jquery.com/download/)

Once you've downloaded the jQuery file you can see it has `.js` extension, because the jQuery is just a JavaScript library, therefore you can include the jQuery file in your HTML document with the [`<script>`](https://www.tutorialrepublic.com/html-reference/html-script-tag.php) element just like you include normal JavaScript files.



```markup
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="utf-8">
    <title>My First jQuery Application</title>
    <link rel="stylesheet" type="text/css" href="/examples/css/style.css">
    <script src="https://code.jquery.com/jquery-3.5.1.min.js"></script>
</head>
<body>
    <h1>Hello, World!</h1>
</body>
</html>
```

Always include the jQuery file before your custom scripts; otherwise, the jQuery APIs will not be available when your jQuery code attempts to access it.

**Tip:** As you can see we've skipped the attribute `type="text/javascript"` inside the [`<script>`](https://www.tutorialrepublic.com/html-reference/html-script-tag.php) tag in the above example. Because this is not required in HTML5. JavaScript is the default scripting language in HTML5 and in all modern browsers.

### Including jQuery from CDN

Alternatively, you can include jQuery in your document through freely available CDN \(Content Delivery Network\) links, if you don't want to download and host jQuery yourself.

CDNs can offer a performance benefit by reducing the loading time, because they are hosting jQuery on multiple servers spread across the globe and when a user requests the file, it will be served from the server nearest to them.

This also offers an advantage that if the visitor to your webpage has already downloaded a copy of jQuery from the same CDN while visiting other sites, it won't have to be re-downloaded since it is already there in the browser's cache.

#### jQuery's CDN provided by StackPath

&lt;script src="https://code.jquery.com/jquery-3.5.1.min.js"&gt;&lt;/script&gt;

You can also include jQuery through [Google](https://developers.google.com/speed/libraries/#jquery) and [Microsoft](http://www.asp.net/ajax/cdn#jQuery_Releases_on_the_CDN_0) CDN's.

### Creating Your First jQuery Powered Web Page

So far you have understood the purposes of jQuery library as well as how to include this in your document, now it's time to put jQuery into real use.

In this section, we will perform a simple jQuery operation by changing the color of the heading text from the default black color to red.

```markup
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="utf-8">
    <title>Example of Simple jQuery Powered Web Page</title>
    <link rel="stylesheet" type="text/css" href="/examples/css/style.css">
    <script src="https://code.jquery.com/jquery-3.5.1.min.js"></script>
    <script>
        $(document).ready(function(){
            $("h1").css("color", "#0088ff");
        });
    </script>
</head>
<body>
    <h1>Hello, World!</h1>
</body>
</html>
```

![](../../../.gitbook/assets/image%20%284%29.png)



