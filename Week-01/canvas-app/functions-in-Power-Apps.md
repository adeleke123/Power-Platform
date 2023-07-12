## Exercise - Get started with functions in Power Apps

When using Microsoft Power Apps, you don't have to write complicated application code the way that a traditional developer does. However, you must express logic in an app and control its navigation, filtering, sorting, and other functionalities. This is where formulas come in.

If you've used Microsoft Excel functions, you should recognize the approach that Power Apps takes. This unit shows a couple of basic formulas for text formatting and then describes three of the formulas that Power Apps includes when it generates an app. With this information, you'll have a better idea of what formulas can do, and then you can also start to write your own.

### Get started with formulas and properties

The previous unit explored controls in all three screens of an app that Power Apps generated. In this section, you’ll modify the properties of the label control to format the item price in the gallery.

By default, the price appears as a plain number without a currency symbol. Suppose that you want to add a dollar sign and change the text color based on the item's cost. For example, red if it's more than $5, but green otherwise. The following graphic shows the expected result.

![image](https://github.com/adeleke123/Power-Platform/assets/51156057/cecb9ca5-02b6-4ea0-86b1-29a1aad82ebe)

By default, Power Apps pulls in a price value for each item. This value is set as the Text property of the label that shows the price.
1. In BrowseScreen1, select the price of the first item. In your Tree view, it's the label control inside of BrowseGallery1 called Subtitle1.
![image](https://github.com/adeleke123/Power-Platform/assets/51156057/ac6f1662-0028-495a-ae89-cbe087074c7b)

2. In the drop-down list of properties, select Text (the default property for a label control).

3. To add the currency symbol for US dollars, set the Text property to this formula:

![image](https://github.com/adeleke123/Power-Platform/assets/51156057/c2762c1a-3be4-43cc-bc38-4ae81739c4fb)

![image](https://github.com/adeleke123/Power-Platform/assets/51156057/7a7c0533-d027-425a-8426-951ce136fbac)

The Text function specifies how to format the number. The formula is like an Excel function, but Power Apps formulas refer to controls and other app elements instead of cells in a workbook.

If you select a control and then open the property drop-down list, a list of properties that are relevant to the control appears. For example, the following is a partial list of the properties for a Label control. Some properties are relevant across a wide range of controls, but others are relevant only for a specific control.

![image](https://github.com/adeleke123/Power-Platform/assets/51156057/b98632e1-8402-4967-adf8-f55c300fed26)

The `Color` property of a label control affects the color of the text. Colors can be portrayed as RGBA, HEX or HTML color names. In our Flooring Estimates app, let's conditionally format the price's color. Select the price label (or Subtitle1), choose the Color property and set it to this formula:

![image](https://github.com/adeleke123/Power-Platform/assets/51156057/70e9acaf-4e3b-4962-b2ad-030d5b7b8801)

Notice how the color of the text was originally an RGBA value equating to the color black, and we changed it to named colors - Color.Red and Color.Green, based on our formula condition. For the formula to work, Power Apps is expecting a value that is a color. As long as your formula provides color data as an output, you can add any working formula as an input.

## Formulas included in the generated app
Power Apps includes formulas in every app that it generates, so let's explore two of them. Both examples are from the browse screen and work with the OnSelect property. This property defines what happens when a user selects a control.

+ The first formula is associated with the IconNewItem1 control new item icon (+). When a user selects this control, the app opens the edit/create screen where they can create an item. To view the formula, let's select the new item icon (+) and then look at the OnSelect property in the formula bar. Place your cursor in the formula bar and you'll see the formula is as follows:

![image](https://github.com/adeleke123/Power-Platform/assets/51156057/a9d8221a-22c5-48e3-ba3e-02b83247e0c9)

The formula instantiates an edit form on the edit/create screen so that users can create an item. A value of `ScreenTransition.None` means that there's no transition, such as a fade, between screens.

+ The second formula is associated with the `IconSortUpDown1` control (button with up and down arrows). The user selects this control to sort the items in the gallery. With the app in edit mode, go ahead and select it. The formula is as follows:

![image](https://github.com/adeleke123/Power-Platform/assets/51156057/8998e50a-58f3-4732-b547-a88d879c33ff)

The formula uses UpdateContext to update a variable called SortDescending1. The exclamation "!" symbol in the formula is a shortcut for the Not function. The value of the variable switches back and forth as you select the control. This variable tells the gallery on this screen how to sort the items, either in descending order or the opposite of descending order.

This app contains many other formulas, so take some time to select different controls and discover the formulas that are currently set for various properties.

For more information about these and other functions, see formula reference for Power Apps page. This page is a good one to bookmark for future use!

For more information on customizing a canvas app, see Use the UI and controls in a canvas app in Power Apps learning path and the Use basic formulas to make a better canvas app in Power Apps learning path.



