# Bootstrap

Bootstrap is a popular CSS framework. It contains pre-written codes for frequently used CSS web features. Bootstrap 5 is the newest version of Bootstrap. In order to use bootstrap, one can access it online or download the whole file to their device(then include the needed set of libraries).

Some components of Bootstrap are the following: navbar, card, alerts, dropdown, containers, and breakpoint.

## Containers in Bootstrap

Containers can be applied by naming the class as “container”. They contain and center the contents placed in them. They also provide margin, padding, alignment and other specifications.

Bootstrap comes with three different containers:

- .container, which sets a max-width at each responsive breakpoint
- `.container-{breakpoint}`, which is `width: 100%` until the specified breakpoint
- `.container-fluid`, which is `width: 100%` at all breakpoints

![container.png](Bootstrap%2097b859640da34558be8de5abe8bb3816/container.png)

## Breakpoints in Bootstrap

Breakpoints determine how your responsive layout behaves across device or viewport sizes in Bootstrap.

![break.png](Bootstrap%2097b859640da34558be8de5abe8bb3816/break.png)

## The Grid System in Bootstrap

It’s used to divide the page into different components displaying different contents. By default, every screen is assumed to have 12 columns. So these columns are divided to contain contents. classes, “row” and “col” are needed for this system to function. 

Example: The following code gives 6 columns if screen is medium and above while it gives full screen for lower screens.

```css
<div class="-col-md-6">
<p> First Paragraph </p>
</div>
```