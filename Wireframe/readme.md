<a name="introduction-wf"></a>
## Introduction: Wireframes 

Wireframes illustrate how the user interfaces with information. A wireframe answers questions as general as _"How does a user access the About page?"_ and as specific as _"What will change on the screen if the user clicks 'submit'?"_ Most wireframes are free of any color or visual design elements, and simply show boxes and lines with notations to outline user interactions.

Wireframes will look different depending on who creates them, but they should always include details about the functionality.

![Wireframe 1](assets/wireframe1.png)
![Wireframe 2](assets/wireframe2.png)
![Projects](assets/projects.png)
![Testimonials](assets/testimonials.png)
![Learn More](assets/learnmore.png)

### Wireframes in the Wild
As a developer, you'll often build pages and sites from wireframes created by User Experience (UX) Designers. Wireframes should detail any and all functionality on the page. If building a website was like building a house, wireframes might be considered the blueprints. They're an important element of communication between the design and engineering teams.

### Want to Create Your Own?

#### Thumbnail Sketches
Wireframing before you build a page or site can be a helpful exercise in planning the functionality and basic layout, especially if your team doesn't have UX Designers. Low-fi wireframes, often called thumbnail sketches, are an easy and quick way to begin. Thumbnail sketches are meant to be drawn quickly, as a way to prototype different layouts for your content. They consist of very simple boxes and lines to represent different elements on the page.

[via sopachu.wordpress.com](https://soapchu.wordpress.com/category/traditional-illustrations/)

#### User Stories
You might also start by creating User Stories. Imagine 3-4 different types of users who will come to your site. Is this a first-time user? A user hesitant to sign up? A user who's been a member of the site for years? How will these personas influence the functionality of your site?

Assuming the identity of these users, ask yourself these questions as you sketch out your site:

- Will the users understand what this product or service does?
- Is the hierarchy of content appropriate for this user's needs?
- Does the user have a clear way to navigate the site from the home page? From all subpages?
- Can the user intuitively interface with the information presented to them?

The best way to see if your site is usable is to test, test, test, test! A simple exercise is to have someone look at wireframes and talk through how they would use the site. Pay close attention to small moments of hesitation or larger moments of confusion, which often reveal issues with the site.

- [A Framework for Modern User Stories](https://medium.com/@jonatisokon/a-framework-for-user-stories-bc3dc323eca9)
- [How to Write a Proper User Story](https://medium.com/paloit/how-to-write-a-proper-user-story-33d939e6f714)

### Tools of the Trade
UX Designers use a number of tools to create wireframes, but basic wireframes can also be done by hand or on a whiteboard. Feel free to try out a few common tools in your spare time!

- [Sketch](https://www.sketchapp.com/)
- [Framer](https://framerjs.com/)
- [Moqups](https://moqups.com/)
- [Adobe Illustrator](http://www.adobe.com/products/illustrator.html)
- [OmniGraffle](https://www.omnigroup.com/omnigraffle)
- [Wireframe.cc](https://wireframe.cc/)

***

<a name="introduction-grids"></a>
## Introduction: Grids 
### Why use a CSS grid?

#### Structure
* Grids are a simple way to apply layout to a webpage. A better layout improves the user experience.
* Grids help avoid stressful CSS debugging by starting out on the right foot.

#### Reusability
* Grids make the layout process easier because of reusable, semantically-named "utility classes" (i.e., a library of CSS class selectors).
* Grids aren't limited to a particular project. We can apply them to pretty much everything we do.
* Grids are highly customizable. You can really make them your own.

_Even if you don't use a grid system, these concepts will translate across other layout problems._

### Basic components of a grid

#### Rows
* The highest-level component of a grid.
* Comprised of columns.

#### Columns
* Contain and separate site content.

#### Gutters
* Provides spacing between our columns. Optional, but useful.

### Opening Exercise

Whiteboard a wireframe for [Craigslist](http://washingtondc.craigslist.org/).

* Focus on the main components of the page: sections that are defined by the rows and columns of our grid.
* Don't worry about site content (e.g., text, images).
* Keep an eye out for width, height, proportion, and number of components.
* [Sample wireframe.](http://www.comentum.com/images/wireframes-sample/ecommerce/home.png)


***

<a name="bootstrap"></a>
## Introduction: CSS Frameworks 

Many workplaces use an established grid system such as Twitter [Bootstrap](http://getbootstrap.com/), [Bulma](https://bulma.io/) [Materialize](https://materializecss.com/) by Google Design or [Semantic UI](https://semantic-ui.com/).

Bootstrap is "the most popular HTML, CSS and JS framework for developing responsive, mobile-first projects on the web."

Features:

1. Grid system
1. Forms/buttons
1. Navigation
1. Tabs and pills
1. Alerts/error messages
1. Modals
1. And much more

Today we will take a look at the grid system that Bootstrap provides. 

Take a look at the [Bootstrap Expo](http://expo.getbootstrap.com/) site to see some examples of sites that use Bootstrap.

#### Setup

To add Bootstrap to a project, use the CDN:

1. Copy-paste the stylesheet `<link>` into the `<head>` of your HTML document before all other stylesheets.
2. Many Bootstrap components require the use of JavaScript to function. Place the following `<script>s` near the end of your pages, right before the closing </body> tag, to enable them.
	
```html
<script src="https://code.jquery.com/jquery-3.3.1.slim.min.js" integrity="sha384-q8i/X+965DzO0rT7abK41JStQIAqVgRVzpbzo5smXKp4YfRvH+8abtTE1Pi6jizo" crossorigin="anonymous"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.14.7/umd/popper.min.js" integrity="sha384-UO2eT0CpHqdSJQ6hJty5KVphtPhzWj9WO1clHTMGa3JDZwrnQq4sF86dIHNDz0W1" crossorigin="anonymous"></script>
<script src="https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/js/bootstrap.min.js" integrity="sha384-JjSmVgyd0p3pXB1rRibZUAYoIIy6OrQ6VrjIEaFf/nJGzIxFDsf4x0xIM+B07jRM" crossorigin="anonymous"></script>
```
3. ALternatively, you may add the starter template provided on the [Bootstrap](https://getbootstrap.com/docs/4.3/getting-started/introduction/) Getting Started website:

```html
<!doctype html>
<html lang="en">
  <head>
    <!-- Required meta tags -->
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">

    <!-- Bootstrap CSS -->
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/css/bootstrap.min.css" integrity="sha384-ggOyR0iXCbMQv3Xipma34MD+dH/1fQ784/j6cY/iJTQUOhcWr7x9JvoRxT2MZw1T" crossorigin="anonymous">

    <title>Hello, world!</title>
  </head>
  <body>
    <h1>Hello, world!</h1>

    <!-- Optional JavaScript -->
    <!-- jQuery first, then Popper.js, then Bootstrap JS -->
    <script src="https://code.jquery.com/jquery-3.3.1.slim.min.js" integrity="sha384-q8i/X+965DzO0rT7abK41JStQIAqVgRVzpbzo5smXKp4YfRvH+8abtTE1Pi6jizo" crossorigin="anonymous"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.14.7/umd/popper.min.js" integrity="sha384-UO2eT0CpHqdSJQ6hJty5KVphtPhzWj9WO1clHTMGa3JDZwrnQq4sF86dIHNDz0W1" crossorigin="anonymous"></script>
    <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/js/bootstrap.min.js" integrity="sha384-JjSmVgyd0p3pXB1rRibZUAYoIIy6OrQ6VrjIEaFf/nJGzIxFDsf4x0xIM+B07jRM" crossorigin="anonymous"></script>
  </body>
</html>
```
		

#### How it works:

Bootstrap includes a responsive, mobile-first fluid grid system that appropriately scales up to 12 columns as the device or viewport size increases.

Page layouts are created through a series of rows and columns that house your content.

Similar to the grid system we created together in class, Bootstrap includes predefined classes for easy layout options:

![](assets/bootstrap_classes.png)

#### Steps to use Bootstrap:

1. Bootstrap requires a containing element to wrap site contents and house our grid system. You may choose one of two containers to use in your projects:
	- Use `.container` for a responsive fixed width container.
	
		```css
		<div class="container">
			...
		</div>
		```
	- Use `.container-fluid` for a full width container, spanning the entire width of your viewport.

		```css
		<div class="container-fluid">
		  ...
		</div>
		```
2. Add rows
	- Use rows to create horizontal groups of columns.
	- Only columns may be immediate children of rows.
	
	```css
	<div class="container-fluid">
		<div class="row">
			(columns)
		</div>
	</div>
	```
3. Add columns
	
	```css
	<div class="container-fluid">
		<div class="row">
		  <div class="col-md-5">.col-md-5</div>
		  <div class="col-md-7">.col-md-7</div>
		</div>
		<div class="row">
		  <div class="col-md-4">.col-md-4</div>
		  <div class="col-md-4">.col-md-4</div>
		  <div class="col-md-4">.col-md-4</div>
		</div>
	</div>
	```
4. Finally, fill in your content

#### Independent Practice :: Restaurant Website

Open [starter-code/restaurant-website](starter-code/restaurant-website) in your text editor. 

For this exercise, you will be tasked with creating a website for a food delivery service with two pages -- a landing page and an ordering page. Make sure the pages are responsive for mobile and tablet viewports.

##### Landing Page User Stories

- User should be able to click both the landing and ordering pages in the navbar
- Click the call to action button that is centered over the hero image and link to the ordering page
- Read the markerting copy in the three-column section
- Read the food delivery service name and tagline and well as click links to both pages
- Read copyright information in the footer 

##### Ordering Page User Stories

- User should be able to click both the landing and ordering pages in the navbar
- User should see that the ordering page is the active item in the navbar
- See the menu on the left side of approximately half the page in a two-column card layout
- See the order on the right side of approximately half the page with a receipt table on top and form below
- Read the food delivery service name and tagline and well as click links to both pages
- Read copyright information in the footer 

***

### Additional Resources

#### Resources
- [Flexbox Grid](http://flexboxgrid.com/)
- [Flexbox in Bootstrap](https://v4-alpha.getbootstrap.com/utilities/flexbox/)
- [Bootstrap](http://getbootstrap.com/)
- [Foundation](http://foundation.zurb.com/)

#### Videos
- [Wireframes in the Design Process](https://generalassembly.wistia.com/medias/lapfitgxmk)

#### Readings
- [All About Grid Systems](https://webdesign.tutsplus.com/articles/all-about-grid-systems--webdesign-14471)