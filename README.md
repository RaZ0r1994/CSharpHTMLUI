# CSharpHTMLUI
This project creates a base for designing forms within a C# application using HTML, CSS and JavaScript. The main reason for that is that HTML gives you endless possibilities to design a UI. Which means that forms are completely customizable. That is something that the default forms can´t provide. If you really want to change the look of your application, you need to override the methods and properties of the forms. That isn´t the easiest and most performant way of creating a UI.

# Setup
After you cloned the project, you need to create a default page. The application will search the default page in the same folder as the executable is in and it should be named 'index.html'.

Here is a template for the index.html
```html
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <meta http-equiv="X-UA-Compatible" content="ie=11">
		<title>TEST</title>
		<meta http-equiv="cache-control" content="no-cache" />
		<script src="https://code.jquery.com/jquery-1.12.4.js"></script>
    </head>

    <body id="body">
		<button id="TESTBUTTON" style="border: red solid 1px; border-radius: 2px;">Click me</button>
		<br/>
		<div style="border: black solid 1px; border-radius: 4px; height: 200px; width: 200px; background-color: grey;">
			<p>test</p>
		</div>
		<div style="border: black solid 1px; border-radius: 4px; height: 200px; width: 200px; background-color: grey; margin: auto;">
			<p>test</p>
		</div>
		
		<script>	
		$(document).click(function(e){
			external.Send(window.event.target.id);
		})
		</script>
	</body>
</html>
```

# Goal
The Goal is to be able to create complete form applications using HTML, CSS and JavaScript which can be deployed onto other devices.

# More Information
As you might be able to see, this Readme is quite empty. So any help with the support is appreciated! Lets see how far this project will go.

