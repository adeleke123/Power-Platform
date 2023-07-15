## More ways to use the navigation function

As previously mentioned, one of the most common ways to move from screen to screen is by setting the OnSelect property of a control. There are also several other ways to trigger the Navigate or Back functions.

## Navigating screens by setting the OnChange property of a drop-down control

One option is to use a DropDown control and an If statement. With this solution, depending on the choice selected in the drop-down menu, the app navigates to a specific screen. If you would like to try this now, you can follow along with the example below (if your VM mode instance is still open from the last exercise you can use that for the following steps).

1. Start an app in Power Apps Studio and add two blank screens. There should be a total of three blank screens.

2. On Screen1, add a Dropdown control.

3. Set the Items property for the Dropdown control to:
```
[" ","Active","Inactive"]

```

4. Set the `OnChange` property for the Dropdown control to the following:

```
If(Dropdown1.Selected.Value ="Active",Navigate(Screen2,ScreenTransition.Cover), If(Dropdown1.Selected.Value = "Inactive",Navigate(Screen3,ScreenTransition.Fade)))
```

On your keyboard, hold the Alt key (or enter app Play mode) to test the new functionality. When you select Active from the drop-down menu, the app should navigate to Screen2. Likewise, if you select Inactive from the same drop-down menu, the app navigates to Screen3. Finally, if you select the blank (" ") option, the app shouldn't navigate to another screen.

## Using variables and the Timer control to navigate screens

You can also use a variable and an If statement to set navigation. Depending on what the app sets the variable value as sends the user to a specific screen. For example, if you have the question "Do you have additional feedback to provide regarding this incident?" If the user selects "Yes", then you want to send the user to the Additional Information screen. If the user selects, "No", then you want to navigate to the Form Completed screen.

Another option is to use a timer control. When the time runs out, the app navigates to a different screen. For example, maybe you only want to allow users 30 seconds to answer the questions on a screen before navigating to the next set of questions.

The following example builds off the previous example and incorporates variables and a Timer control.

1. On Screen1, add a Timer control.

2. Set the Duration property to 10000 (in milliseconds)

3. Set the Auto start to On (select the toggle in the properties pane on the right side of the screen).

4. Set the OnTimerEnd property to:

```
If(Dropdown1.Selected.Value = " ",Navigate(Screen2))

```
5. Select the drop-down control and modify the `OnChange` property to

```
If(Dropdown1.Selected.Value = "Active",Set(varStatus,1),If(Dropdown1.Selected.Value ="Inactive",Set(varStatus,2),Set(varStatus,0)))

```
6. Add a new Button control, position it under the drop-down menu, and set the Text property to "Next".

7. Set the `OnSelect` property for the "Next" button to
```
If(varStatus = 1,Navigate(Screen2,ScreenTransition.Cover),
If(varStatus = 2,Navigate(Screen3,ScreenTransition.Fade)))
```
8. There are now two ways to navigate to other screens from Screen1. Put your app in play mode. You'll notice that the timer begins counting right away and nothing will happen unless the empty/blank field is selected in your drop-down. Select the empty/blank field from your drop-down. If you already have it selected, or if you select it before the timer expires, your app will navigate to Screen2. If your timer runs to 10 seconds before you can change the dropdown, then you can select the timer control to restart the timer.

9. Return to Screen1 by selecting Back. Now let's try the alternate means of navigation. Select Active from the drop-down menu, and this will set your variable named varStatus to 1. Then when you select the "Next" button, you'll land on Screen2. Notice how your timer starts again the moment you return to Screen1, but it will not navigate to Screen2 unless your drop down is on the empty/blank field.

10. Go back to Screen1 and now select Inactive from the same drop-down. This makes your value of varStatus 2, and then pressing the "Next' button navigates you to Screen3.

## Documentation Screen
Before moving to the knowledge check, let's discuss the Documentation screen. You can add a screen to your app and rename the screen Documentation. With no Navigation pointing to this screen, it isn't accessible to your end-users. The purpose of this screen is to give the App creator or co-editors a location in the app to make notes or add documentation about certain aspects of how the app functions. It can be a place to keep track of settings, such as formatting or colors. Using a Documentation screen is a great technique to provide instructions to other developers of the app.

## Summary
There are different and flexible ways to configure navigation in your app. In the first example, the navigation dynamically changed with user input to the drop-down control. In the second example, we used navigation in two different ways: via the timer reaching zero, or by selecting a button. The variable allowed you to control which screen your user navigated to, based on the drop-down value selected, and triggered when the user selected a button control. A Documentation screen in your app that users can't navigate to provides developers a location to add notes on the app. Power Apps provides the flexibility to choose what works best for your solution!




