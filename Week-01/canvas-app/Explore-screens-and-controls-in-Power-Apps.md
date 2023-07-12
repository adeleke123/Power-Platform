## Explore screens and controls in Power Apps

This unit examines the screens and other controls that define the behavior of apps that Microsoft Power Apps generates. All the details won't be covered; however, knowing more about how these apps work will help you build your own apps.

## Controls in Power Apps
A control is a UI element that produces an action or shows information. Many controls in Power Apps are similar to controls that you've used in other apps: labels, text-input boxes, drop-down lists, navigation elements, and so on.

In addition to these typical controls, Power Apps has more specialized controls, which you can find on the + Insert tab, which includes a search field to help you find what you're looking for.

![image](https://github.com/adeleke123/Power-Platform/assets/51156057/20aef55b-6fdf-4bc1-b5e2-1ffaa9bd2345)

A few controls that can add interest and impact to your apps include:

+ Galleries - Controls that are layout containers that hold a set of controls that show records from a data source.
+ Forms - Controls that show details about your data and let you create and edit records.
+ Media - Controls that let you add background images, include a camera button (so that users can take pictures from the app), a barcode reader for quickly capturing identification information, and more.
+ Charts - Controls that let you add charts, including Power BI data, so that users can perform instant analysis of their data.
To see what controls are available, select the + Insert tab, and then expand the different fields. As you do, you'll see the utility of the search field to assist you in quickly finding what you're looking for. Try entering a few values in the search field to see the behavior.

## Explore the browse screen
Each screen in the app has multiple controls, but one control takes up most of the screen space. If we can return to the Flooring Estimates app that we generated in the previous module for a moment, we'll examine the content created by Power Apps when we created that app.

The first screen in the app is the browse screen, which is named BrowseScreen1 by default. Some of the other controls in the browse screen that you'll want to become familiar with include:

+ BrowseGallery1 - A control that takes up most of the screen and shows data from your data source.

+ NextArrow1 - A control that is inside of BrowseGallery1 and that, when selected, opens the details screen.

+ IconNewItem1 - When this control is selected, it opens the edit screen to create a new item.

![image](https://github.com/adeleke123/Power-Platform/assets/51156057/e014bdcc-b810-45b8-a69b-707fb169ca81)

## Explore the details screen
The details screen is named DetailScreen1 by default. Notable controls include:

+ DetailForm1 - A Form control that contains other controls and contains a data card for each field of the record that is being displayed.

+ Name_DataCard1 - A Card control, automatically created when a form is added into your app. Each card represents a single field of the record. In this case, it shows a flooring category from the Flooring Estimates table, as shown in the previous unit.

+ IconEdit1 - A control that opens the edit/create screen so that the user can edit the current item.

![image](https://github.com/adeleke123/Power-Platform/assets/51156057/69a3db2f-f338-4125-a0d5-46272baad7e3)

## Explore the edit screen
The third screen in the app is EditScreen1. Notice how these controls allow your user to edit the item portrayed, via text input fields and some prompting dialog over the image. Even though you see similar controls to the browse screen, the properties of these controls are different. Some of the edit screen controls include:

+ EditForm1 - A Form control containing other controls, and it contains a data card for each field of the record that is being edited.

+ Category_DataCard2 - A card control that shows a flooring category from the Flooring Estimates table.

+ IconAccept1 - A control that saves the user's changes when selected.

![image](https://github.com/adeleke123/Power-Platform/assets/51156057/9f46d752-ef15-4731-b941-0aa01931eedd)
With this introduction to the new screens and controls, we can learn about using some functions in Power Apps in the next unit.
