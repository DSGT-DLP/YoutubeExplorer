# Youtube Explorer Frontend

As part of the frontend, our app will simply have the search bar as the main entity that the user can interact with. 

If you go into `src/App.js`, you will see some code that is responsible for spinning up the view you saw in the setup.

## Important Frontend Files
* `/src/components` (file that contains the building blocks of the user view)
   * `index.js` --> Don't worry about this file. This helps make sure that `App.js` is able to display the building blocks of the frontend
   * `Title.js` --> shows the title text. See where "Youtube Explorer" appears in this file and try tweaking it around
   * `Search.js` --> controls the rendering of the text field for entering Youtube Channel + Search Button
   * `Result.js` --> controls rendering of result table 

Right now, the view is a bunch of text and we can surely improve the aesthetics!

## Quick Cleanups on the View
1. You might be noticing that the "Youtube Explorer" Title text is scootched all the way to the left hand side of the screen. Find a way to make the "Youtube Explorer" title text centered on the screen (hint: this should only involve changing one line of code)

2. Currently, our app displays all entities (header, text) in a vertical fashion. Sometimes, we might want entities (eg: buttons, text fields, tooltips, etc) on the "same level" in the screen (imagine two buttons next to each other on a website). Find a way to display the "Put text field to enter Youtube Channel here!" and "Put search button here!" on the same level instead of aligned vertically

## Execution Steps (Recommended)
1. Implement `Search.js`
2. Follow instructions in `BACKEND.MD`
3. Implement `Result.js` (once you know how the data from the backend will be structured, making the table should be a bit more doable)