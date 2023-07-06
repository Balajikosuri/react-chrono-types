React Chrono | Reading Material
Concepts in Focus
Third-Party Package react-chrono
Advantages
Chrono Props
mode
items
theme
Rendering Custom Content
Reference
1. Third-Party Package react-chrono
NPM contains a react-chrono, a third-party package to display the timeline in your application.

It provides a React component Chrono to build a timeline that displays events chronologically.

Installation Command:

1.1 Advantages
Can render the timelines in three different modes (horizontal, vertical, and tree).
Can autoplay the timeline with slideshow mode.
Can navigate the timeline via keyboard.
2. Chrono Props
We can provide different props to the ReactJS Chrono component. Below are some of the most commonly used props.

Prop	Description	Default Value
mode	Sets the mode of the component	'HORIZONTAL' (value can be 'HORIZONTAL', 'VERTICAL' or 'VERTICAL_ALTERNATING')
items	Collection of Timeline Item Model	[]
theme	Customises the colors	No default value
2.1 mode
Example:

JSX
2.2 items
The items prop is used to build the timeline. It is a collection of the Timeline Item Model.

Timeline Item Model is an object consist of the given properties:

Name	Description	Type
title	title of the timeline item	String
cardTitle	title of the timeline card	String
cardSubtitle	text of the timeline card	String
cardDetailedText	detailed text of the timeline card	String or String[]
media	media object to set image or video	Object
Example:

CSS
 
JSX
Collapse
Output:

A single timeline item is created with the values of the Timeline Item Model in the items prop.


Warning
If any property misses in the Timeline Item Model, the respective value won't be displayed in the timeline item.

Note
The Chrono Component should be wrapped in a container that has a width and height.
2.3 theme
The colors can be customized with the theme prop.

Example:

JSX
3. Rendering Custom Content
The custom content can be inserted by just passing the elements between the Chrono tags.

Example:

The below example will create two timeline items.

CSS
 
JSX
Collapse
Output:

Each HTML div element is automatically converted into a timeline item and inserted into the timeline card.


Note
The items prop is optional and custom rendering is supported on all three modes.
Example:

The below example will set the title for the custom contents.

CSS
 
JSX
Collapse
Output:


4. Reference
To know more about the react-chrono, you can refer to this.
