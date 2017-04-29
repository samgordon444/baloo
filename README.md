# Baloo v1.3
A simple bare necessities responsive CSS grid setup

## Intro
As a designer who uses Sketch for all interface design, I have a starting point every time I create a new UI - the layout grid is built in, ready to go. When I transition to coding my site, the grid isn't there, so I either have to spend time creating one to fit my design or selecting a boilerplate, which then takes time to be stripped back. I was in need of a boilerplate that had zero type styles, zero color styles, just the grid. JUST. THE. GRID. And maybe also normalize.css because it's great. This is meant for the designer who codes and wants to transition lightning fast from concept to product, with maximum control over their pixel-perfect design from the very beginning.

So that's what we have here. Just the grid, set by default at 1200px wide with 15px outside gutters, 30px inside gutters, and 70px columns. Rows have 0 top and bottom margins because even that can be an unnecessary design element that ends up being deleted. To top it off, the CSS file is only 5KB, smaller than most "super teeny tiny minimal boilerplates".

## Install
Link `baloo.css` to your html file, and put all other styles in a separate CSS file.

To change the total width of the container, change the `max-width` style of `.container`
This total width value is calculated as: `outside gutters (15px) + inside gutters + columns`. So if you want the width of your content to be 1170px, the `max-width` (which includes the two outside gutters) should be set at 1200px. To change the outside gutter, edit the padding of `.container`

## Use
Wrap the main content in a div with `class="container"`

Each horizontal section (or row) of content should be wrapped in a div with `class="row"`

Then simply add `class="_NUMBER_ columns"` to divs within row, using column names below.<br> 
EX: <code>&lt;div class="three columns"&gt;&lt;/div&gt;</code>

To offset columns, use the offset class names below. <br>
EX: <code>&lt;div class="six columns offset-two"&gt;&lt;/div&gt;</code>

The overall structure looks like this:
<code><pre>&lt;div class="container"&gt;
  &lt;div class="row"&gt;
    &lt;div class="three columns&gt;&lt;/div&gt;
    &lt;div class="nine columns"&gt;&lt;/div&gt;
  &lt;/div&gt;
&lt;/div&gt;</pre></code>

### Column class names:
one column<br>
two columns<br>
three columns<br>
four columns<br>
five columns<br>
six columns<br>
seven columns<br>
eight columns<br>
nine columns<br>
ten columns<br>
eleven columns<br>
twelve columns<br>
one-third column<br>
two-thirds column<br>
one-half column

### Column offset class names:
offset-one<br>
offset-two<br>
offset-three<br>
offset-four<br>
offset-five<br>
offset-six<br>
offset-seven<br>
offset-eight<br>
offset-nine<br>
offset-ten<br>
offset-eleven<br>
offset-one-third<br>
offset-two-thirds<br>
offset-one-half
