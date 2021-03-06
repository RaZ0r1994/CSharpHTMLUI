# CSharpHTMLUI
This project creates a base for designing forms within a C# application using HTML, CSS and JavaScript. The main reason for that is that HTML gives you endless possibilities to design a UI. Which means that forms are completely customizable. That is something that the default forms can´t provide. If you really want to change the look of your application, you need to override the methods and properties of the forms. That isn´t the easiest and most performant way of creating a UI.

# Setup
After you cloned the project, you need to create a default page. The application will search the default page in the same folder as the executable is in and it should be named 'index.html'.

The HTML pages have to contain 
- &lt;!--Meta:Info:--&gt;
- &lt;!--Name:index.html:--&gt;

above the DOCTYPE and 
- &lt;!--EOF--&gt;

in the last line of the file.

Here is an example for the index.html
```html
<!--Meta:Info:-->
<!--Name:index.html:-->
<!DOCTYPE html>
<html lang="en">

    <head>
        <meta charset="UTF-8"/>
        <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
        <meta http-equiv="X-UA-Compatible" content="ie=11"/>
		<title>TEST</title>
		<meta http-equiv="cache-control" content="no-cache" />
		<script src="https://code.jquery.com/jquery-1.12.4.js"></script>

        <script>
		$(document).click(function(e){
			external.Send(window.event.target.id);
            })
        </script>
    </head>

    <body id="body">
	<button id="TESTBUTTON" style="border: red solid 1px; border-radius: 2px;">Click me</button>
	<br/>
	<div style="border: black solid 1px; border-radius: 4px; height: 200px; width: 200px; background-color: grey;">
		<p id="coolDemo">test</p>
	</div>
		<div style="border: black solid 1px; border-radius: 4px; height: 200px; width: 200px; background-color: grey; margin: auto;">
		<p>test</p>
	</div>
	</body>
</html>
<!--EOF-->
```


# First Todo´s
- ~~Add control caching for fast UI changes~~
- ~~Implement the site-name in the html to be able to re-generate html from resources~~
- Add encryption to the rebuild, minified, html pages
