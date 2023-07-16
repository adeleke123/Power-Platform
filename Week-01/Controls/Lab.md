## Lab - Create a canvas app with unique controls

## Creating the collection of data
In this training, you will use multiple controls mentioned in the previous units to create a unit canvas app that will change as you interact with the controls. This will give you an idea of the capabilities of controls and how you can fit them to your needs.

+ Sign-in to Power Apps. If using the virtual environment, skip to step 2.

+ On the Home screen, select Canvas app from blank.

![image](https://github.com/adeleke123/Power-Platform/assets/51156057/b846c677-af8b-47c3-8ea1-0d5bb2d19edb)

![image](https://github.com/adeleke123/Power-Platform/assets/51156057/58090a1d-c827-44fa-b337-d849cdb3d637)

+ Select the Insert tab and add a button, and set its OnSelect property to this formula:

```
 ClearCollect(CityPopulations, {City:"London", Country:"United
 Kingdom", Population:8615000}, {City:"Berlin",
 Country:"Germany", Population:3562000}, {City:"Madrid",
 Country:"Spain", Population:3165000}, {City:"Rome",
 Country:"Italy", Population:2874000}, {City:"Paris",
 Country:"France", Population:2273000}, {City:"Hamburg",
 Country:"Germany", Population:1760000}, {City:"Barcelona",
 Country:"Spain", Population:1602000}, {City:"Munich",
 Country:"Germany", Population:1494000}, {City:"Milan",
 Country:"Italy", Population:1344000})

```
![image](https://github.com/adeleke123/Power-Platform/assets/51156057/16032585-87ec-442e-a7f5-a5497089b2e4)

+ Press and hold Alt Key, and select the Button control. (This will create your collection and store all the information.).

+ Select the Gallery dropdown at the top and choose Blank vertical gallery and choose CityPopulations from the data source pop-up.

+ With the gallery selected, in the right pane, change the layout from blank to Title, subtitle, and body.

+ Select the last or third Label in the first item of the gallery, and change the Text property to ThisItem.Population.

![image](https://github.com/adeleke123/Power-Platform/assets/51156057/7743beb4-0870-47af-9100-a7d5de57feb8)

+ Select the Input dropdown and choose Slider.

+ Change the Maximum property of the slider to 10000000.

+ Insert a Label and change the Text property to Slider1.Value.

+ Select the first item in the gallery, and select Icons from the top bar and choose the Check.

+ Change the Visible property of the check icon to:

```
ThisItem.Population > Slider1.Value
```

![image](https://github.com/adeleke123/Power-Platform/assets/51156057/79e9b052-4b2d-44c5-9c0a-b9ed8dea7e88)

As you change the slider, you should see check marks appear and disappear per item in the gallery since you set the visibility to change depending on the slider control. Essentially, you made a gallery that shows whether a city's population is greater or not than the slider value. Here is a video of all the controls in action.


