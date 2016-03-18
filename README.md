# Baloo
A simple, bare-necessities responsive CSS grid setup

As a designer who uses Sketch for all interface design, I have a starting point every time I create a new UI - the layout grid is built in, ready to go. When I transition to coding my site, the grid isn't there, so I either have to spend time creating one to fit my design or selecting a boilerplate, which then takes time to be stripped back. I was in need of a boilerplate that had zero type styles, zero color styles, just the grid. JUST. THE. GRID. And maybe normalize.css because it's great.

So that's what we have here. Just the grid, set by default at 1200px wide with 10px outside gutters, 20px inside gutters, and 80px columns. Rows have 0 top and bottom margins because even that can be an unnecessary design element that ends up being deleted. To polish it off, the file is minified to less than 4KB.

# Use Baloo
Link baloo.css to your html file, and put all other styles in a separate CSS file.
