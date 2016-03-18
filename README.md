<style>/* normalize.css v3.0.3 | MIT License | github.com/necolas/normalize.css */img,legend{border:0}legend,td,th{padding:0}html{font-family:sans-serif;-ms-text-size-adjust:100%;-webkit-text-size-adjust:100%}body{margin:0}article,aside,details,figcaption,figure,footer,header,hgroup,main,menu,nav,section,summary{display:block}audio,canvas,progress,video{display:inline-block;vertical-align:baseline}audio:not([controls]){display:none;height:0}[hidden],template{display:none}a{background-color:transparent}a:active,a:hover{outline:0}abbr[title]{border-bottom:1px dotted}b,optgroup,strong{font-weight:700}dfn{font-style:italic}h1{font-size:2em;margin:.67em 0}mark{background:#ff0;color:#000}small{font-size:80%}sub,sup{font-size:75%;line-height:0;position:relative;vertical-align:baseline}sup{top:-.5em}sub{bottom:-.25em}svg:not(:root){overflow:hidden}figure{margin:1em 40px}hr{box-sizing:content-box;height:0}pre,textarea{overflow:auto}code,kbd,pre,samp{font-family:monospace,monospace;font-size:1em}button,input,optgroup,select,textarea{color:inherit;font:inherit;margin:0}button{overflow:visible}button,select{text-transform:none}button,html input[type=button],input[type=reset],input[type=submit]{-webkit-appearance:button;cursor:pointer}button[disabled],html input[disabled]{cursor:default}button::-moz-focus-inner,input::-moz-focus-inner{border:0;padding:0}input{line-height:normal}input[type=checkbox],input[type=radio]{box-sizing:border-box;padding:0}input[type=number]::-webkit-inner-spin-button,input[type=number]::-webkit-outer-spin-button{height:auto}input[type=search]{-webkit-appearance:textfield;box-sizing:content-box}input[type=search]::-webkit-search-cancel-button,input[type=search]::-webkit-search-decoration{-webkit-appearance:none}fieldset{border:1px solid silver;margin:0 2px;padding:.35em .625em .75em}table{border-collapse:collapse;border-spacing:0}
/* baloo.css v1.1 | MIT License | github.com/samgordon444/balooCSS */.column,.columns,.container{width:100%;box-sizing:border-box;margin-left:0;}.container{position:relative;max-width:1220px;margin:0 auto;padding:0 10px}.column,.columns{float:left}@media (min-width:450px){.column,.columns{margin-left:1.6936%}.column:first-child,.columns:first-child{margin-left:0}.one.column,.one.columns{width:6.78%}.two.columns{width:15.255%}.three.columns{width:23.73%}.four.columns{width:32.204%}.five.columns{width:40.678%}.six.columns{width:49.153%}.seven.columns{width:57.628%}.eight.columns{width:66.103%}.nine.columns{width:74.577%}.ten.columns{width:83.052%}.eleven.columns{width:91.526%}.twelve.columns{width:100%;margin-left:0}.one-third.column{width:32.204%}.two-thirds.column{width:66.103%}.one-half.column{width:49.153%}.offset-one.column,.offset-one.columns{margin-left:8.4736%}.offset-two.column,.offset-two.columns{margin-left:16.9472%}.offset-three.column,.offset-three.columns{margin-left:25.4208%}.offset-four.column,.offset-four.columns{margin-left:33.8944%}.offset-five.column,.offset-five.columns{margin-left:42.368%}.offset-six.column,.offset-six.columns{margin-left:50.8416%}.offset-seven.column,.offset-seven.columns{margin-left:59.3152%}.offset-eight.column,.offset-eight.columns{margin-left:67.7888%}.offset-nine.column,.offset-nine.columns{margin-left:76.2624%}.offset-ten.column,.offset-ten.columns{margin-left:84.736%}.offset-eleven.column,.offset-eleven.columns{margin-left:93.2096%}.offset-one-third.column,.offset-one-third.columns{margin-left:33.8976%}.offset-two-thirds.column,.offset-two-thirds.columns{margin-left:67.7966%}.offset-one-half.column,.offset-one-half.columns{margin-left:50.8466%}.offset-one:not(:first-child){margin-left:10.1672%}.offset-two:not(:first-child){margin-left:18.6408%}.offset-three:not(:first-child){margin-left:27.1144%}.offset-four:not(:first-child){margin-left:35.588%}.offset-five:not(:first-child){margin-left:44.0616%}.offset-six:not(:first-child){margin-left:52.5352%}.offset-seven:not(:first-child){margin-left:61.0088%}.offset-eight:not(:first-child){margin-left:69.4824%}.offset-nine:not(:first-child){margin-left:77.956%}.offset-ten:not(:first-child){margin-left:86.4296%}.offset-eleven:not(:first-child){margin-left:94.9032%}.offset-one-third:not(:first-child){margin-left:35.5912%}.offset-two-thirds:not(:first-child){margin-left:69.4902%}.offset-one-half:not(:first-child){margin-left:52.5402%}}.container:after,.row:after,.u-cf {content: "";display: table;clear: both; }</style>

# Baloo
A simple bare necessities responsive CSS grid setup

As a designer who uses Sketch for all interface design, I have a starting point every time I create a new UI - the layout grid is built in, ready to go. When I transition to coding my site, the grid isn't there, so I either have to spend time creating one to fit my design or selecting a boilerplate, which then takes time to be stripped back. I was in need of a boilerplate that had zero type styles, zero color styles, just the grid. JUST. THE. GRID. And maybe also normalize.css because it's great. This is meant for the designer who codes and wants to transition lightning fast from concept to product, with maximum control over their pixel-perfect design from the very beginning.

So that's what we have here. Just the grid, set by default at 1220px wide with 10px outside gutters, 20px inside gutters, and 80px columns. Rows have 0 top and bottom margins because even that can be an unnecessary design element that ends up being deleted. To polish it off, the file is minified to less than 5KB, smaller than most "super teeny tiny minimal boilerplates".

# Install
Link baloo.css to your html file, and put all other styles in a separate CSS file. Alternatively, you could add lines 3 and 4 of baloo.css into the head of your HTML. It's only two lines for a reason.

To change the total width of the container, change the max-width style of .container
This total width value is calculated as: Outside gutters (10px) + inside gutters + columns. So if you want the width of your content to be 1200px, the max-width (which includes the two outside gutters) should be set at 1220px. To change the outside gutter, edit the padding of .container

# Use
Wrap the main content in a div with class="container"

Each horizontal section (or row) of content should be wrapped in a div with class="row"

Then simply add class="_NUMBER_ columns" to divs within row, using column names below.<br> 
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

Column class names:<br>
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

Column offset class names:<br>
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
