## The navigation and back function

In the previous section, you learned how to implement the Navigate and Back functions using a Control. When employing these functions, like any other function in Power Apps, we need to define certain arguments.

## Navigate function
Here's a breakdown of the Navigate syntax:

Navigate(Screen [, Transition [, UpdateContextRecord ]])

Screen - Required. The screen to display.

ScreenTransition - Optional. The visual transition to use between the current screen and the next screen. The default value is None.

UpdateContextRecord - Optional. A record that contains the name of at least one column and a value for each column. This record updates the context variables of the new screen as if passed by the UpdateContext function.

In the first argument, you specify the name of the screen to navigate to. In the second argument, you specify how the old screen visually changes to the new screen. In the third argument, you can specify a Context variable.

Let's take a closer look at the second argument, ScreenTransition. Below is a list with descriptions of the different ScreenTransitions you could apply. Each ScreenTransition produces a slightly different visual experience for the user, and the transitions all occur in a split second.

Screen transitions
ScreenTransition.Cover - The new screen slides into view from right to left, covering the current screen.

ScreenTransition.CoverRight - The new screen slides into view from left to right, covering the current screen.

ScreenTransition.Fade - The current screen fades away to reveal the new screen.

ScreenTransition.None - (Default) - The new screen quickly replaces the old screen.

ScreenTransition.UnCover - The current screen slides out of view from right to left, uncovering the new screen.

ScreenTransition.UnCoverRight - The current screen slides out of view from left to right, uncovering the new screen.
