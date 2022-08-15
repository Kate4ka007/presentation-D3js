Hello! Today I want to tell you about D3.js. 
D3.js is an open source JavaScript library that
allows you to create dynamic data visualizations in web browsers using HTML5 and CSS.
D3.js specializes in presenting large datasets in a user-friendly and interactive way.

D3.js visualizations are created entirely using JavaScript. This allows frontend developers to add advanced data visualization to their interfaces without learning a new language. D3.js has built-in chart styles for everything from a simple pie chart to an interactive pie chart.

Here are some beautiful examples.
What is data visualization for?
Data visualization helps to:
- Make quick decisions based on large datasets
- Understand the main market trends
- Get information at a glance
- Find errors in recorded data

Top Features of D3.js:					
 - Uses the established standards SVG, HTML and CSS to make it compatible with existing technologies.
 - D3 can use static data or fetch it from remote servers in several formats like Arrays, Objects, CSV, JSON, or XML.
 - D3 allows you to manipulate the Document Object Model (DOM) using your data.
 - D3 provides dynamic properties and elements. Your data defines the style of your visualization.	

 - D3 features dozens of built-in graph formats for common applications like ranking, correlation, and distribution.
 - D3 allows you to create custom visualizations from scratch or by tweaking current graph formats.
 - D3 provides built-in animation functions the transition(), duration(), delay() and ease() functions, which automatically animate features of your graph based on user interaction, timed transitions, or other events.

How to install D3.js?
	You can use the D3 library by linking it directly to your HTML page from the Content Delivery Network. 	Using CDN will allow you to work with D3 without downloading the source code: 	

Fundamental components of D3.js
  Selections, used to select DOM elements for manipulation.
  DOM manipulation, used to add or modify text within DOM elements.
  Method Chaining, used to create a pipeline of methods that each transform an object.
  Data Joins, used to bind data to a selected element to make data-based manipulations easier.


We don't have much time, so I'll talk about the main methods we work with in D3.js first.

D3 Selections
  Selection is the beginning of most D3 method chains as it dictates which elements will be affected by later methods.
  There are two methods for selection in D3.js, select() and selectAll().

The select() method is used to select a single instance of a given HTML tag.
  If multiple instances of the selected tag are present, then it will select the first element only. 

The other method for selection is selectAll() which allows you to select multiple instances of an HTML tag. If multiple instances are present, it will select all of them. First, we select p tag using the selectAll() method. Then we  use the style() method to add style to selected text.

In D3.js we can manipulate the DOM
Now we’ll take a look at the most common DOM manipulation methods		
	text()
  append()
  remove()
  style()
  attr() 

The text() method manipulates DOM elements and is generally used to add or modify the text inside DOM elements. We first use the select() method to select div elements. Then we use the text() method to add our text to the div element.


The append() method is used to add a new HTML element the selected element. We use the append() method to add a new p element in div element. Then, we have added the text “Bye” using the text() method.


The remove() method is used to remove a selected HTML element. The select() method selects the first div element. Then, we use the remove() method to remove the selected element. By the end, only the second and third div element is shown.


D3.js provides the style() method to set the style of selected DOM elements. The first parameter of style is always the attribute you want to edit and the second parameter is the new value. Style() method can only change a single attribute.


Instead of calling style() twice, we can call attr() once. The attr() method links your element to a CSS style sheet and applies the sheet’s settings to any selected elements.

Now let's talk about svg in D3.js
What is SVG?
SVG is an image that is text-based and it is similar in structure to HTML.
SVG sits in the DOM, properties can be specified as attributes.
SVG should have absolute positions relative to the origin.


We can create svg using D3.js
First we will create two constants with height and width values, then using the select method, we select the body, insert svg into it and add the height and width attributes. Save the file.
And now we can see inside the body our svg sized 400 by 200


This is a simple example of a bar chart that we can make.

Now you should understand this code a little.
We are creating an svg with attributes inside the body.
Next we work with svg.
In svg, we select rect - these are rectangular svgs.
The data() method is used to specify which data we will be using.
The enter() method creates an initial data connection with the elements, and now we can create a rectangular svg for each element of our data array.
Based on the index of the element in our data array,
we shift each element along the x-axis and add the distance between them. Then based on our data we set the height of our columns,  we will multiply each element by 3 for better visualization.
Add a blue fill and class to each, add a title.
and then in each title we add a value based on our data and set their position.

As a result, we get a rectangular svg with other svgs inside based on each member of the data array,
each element has a title with a value.

That's all for me.
More information you can see on the official website of d3.js
Bye!
			  
https://youtu.be/Q55hX77c3Hc

https://youtu.be/Q55hX77c3Hc