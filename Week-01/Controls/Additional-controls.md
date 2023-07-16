## Additional controls for enhancing your app's usability

At the beginning of the module, you learned what controls are, when to use them, and how to modify control properties. In this section, you get a more detailed look into some of the controls available from the Controls drop-down menu in the ribbon. On the Insert tab, if you select the Input heading, you will get a list of several different controls.

![image](https://github.com/adeleke123/Power-Platform/assets/51156057/e014ba90-dd29-40eb-96a7-2064609d9730)

Remember, every control was designed with different use cases in mind. The following information about a few of the controls will help you to decide when you might use each one.

## Controls with pre-populated values
Each of these controls allows you to determine the values the user can select from. Use these controls when you want to control the values for your data set. This is often an important consideration for reporting. As a trade-off, you may miss valuable insights that come from free form answers. Here's a closer look at the differences between each of these controls.

+ Drop down - This control conserves screen real estate, especially when the list contains a large number of choices. The control takes up only one line unless the user selects the chevron to reveal more choices. This control will show a maximum of 500 items.

+ Combo box - This control allows you to search for items you will select. The search is performed on the server on the SearchField property so performance is not affected by very large data sources.

+ List box - This control always shows all available choices (unlike a Dropdown control) and in which the user can choose more than one item at a time (unlike a Radio control).

+ Check box - A control that the user can select or clear to set its value to true or false. The user can specify a Boolean value by using this familiar control.

+ Radio - A Radio control, a standard HTML input control, is best used with only a few, mutually-exclusive options.

## Controls for ratings
When you have a specific need for the app users to rate items, the following two controls provide a better experience than free form text or drop-down controls.

+ Slider - The user can indicate a value, between a minimum and a maximum value that you specify, by dragging the handle of a slider left-right or up-down, depending on the direction that you choose.

+ Rating - In this control, the user can indicate, for example, how much they liked something by selecting a certain number of stars.

## Other available controls
+ Toggle - Use this control to enhance the UI of the app. It functions in the same manner as the check box control.

+ Timer - A control that can determine how your app responds after a certain amount of time passes. For example, determine how long a control appears or navigate to another screen after a certain amount of time has passed.

+ Date Picker - A control that allows you to select a Date from a calendar.

+ Button - Configure the OnSelect property of a button control to run one or more formulas when the user clicks or taps the control. The button control is frequently used to submit data to the data source.
