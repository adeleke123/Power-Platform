## Understanding navigation

In Power Apps, because most apps have multiple screens, it's essential that you understand how to implement the Navigate function in your app. The Navigate function allows users to go (or navigate) from screen to screen within an app. For example, if you create an app with three screens and you want to give users a way to go to another screen, set the OnSelect property of a Button control to:

`Navigate(Screen2,ScreenTransition.Cover)`

When a user selects this button, they automatically go to `Screen2`. You could also use this formula in the OnSelect property of an icon, such as an arrow, or you could use it in the `OnSuccess property` of a form. Navigate can be used in any place where you want to provide a user with the ability to go to a specified screen.

The Navigate function also allows for a visual transition as the user goes to another screen, by using the `ScreenTransition` parameter. In the example shown above, we used `ScreenTransition.Cover`. There are a few different ScreenTransitions to choose from, and each one provides a slightly different user experience when navigating screens. ScreenTransitions will be covered in further detail later in this module.

Another screen navigation function is the `Back() function`. The `Back() function` navigates the user to the last screen they were working on. The main difference here's with Navigate, you have the user go to a specific screen, and with Back, the app could go to any screen that the user was using immediately before landing on the current screen.

When you use Navigate, you can also set one or more context variables to pass parameters to another screen. If you've used another programming tool, this is similar to passing parameters to procedures.

### Hidden screens

You can have "Hidden screens" in your app for various purposes, such as:

+ Documentation screen

+ Settings screen

+ Special permissions screen

A `Hidden screen` allows the creator of the app to add screens but not give users access those screens. You can accomplish hidden screens by not creating any navigation for users to get to those screens. There's an example later in this module to demonstrate this functionality further.

