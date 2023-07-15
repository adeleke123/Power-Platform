## More ways to use the navigation function

As previously mentioned, one of the most common ways to move from screen to screen is by setting the OnSelect property of a control. There are also several other ways to trigger the Navigate or Back functions.

Navigating screens by setting the OnChange property of a drop-down control
One option is to use a DropDown control and an If statement. With this solution, depending on the choice selected in the drop-down menu, the app navigates to a specific screen. If you would like to try this now, you can follow along with the example below (if your VM mode instance is still open from the last exercise you can use that for the following steps).

Start an app in Power Apps Studio and add two blank screens. There should be a total of three blank screens.

On Screen1, add a Dropdown control.

Set the Items property for the Dropdown control to:
