## Learn about mobile-optimized apps

When you design and create a mobile-optimized canvas app from Power Apps, you'll need to consider several design components.

A mobile-optimized canvas app should have the following design characteristics:

A clearly defined purpose

A responsive design [Bring your own device (BYOD)]

Simplistic user interface

Intuitive navigation

External peripherals aren't required

Offline capabilities

Connectivity alerts

Seamless setup

Optimized for performance

Clearly defined purpose
A mobile-optimized application should have a clearly defined purpose. When people use apps in a mobile capacity, the fewest actions that are required to accomplish the task will directly correlate to a better user experience.

Determine if you want a single app with many different actions, such as a mobile warehouse application that will do all actions for maintaining inventory, or a single application for a specific purpose, such as creating customers. Then, ask yourself the following clarifying questions:

Is it easier to navigate back to a home page to complete different actions, or is it easier to exit the app to complete another action?

Is it a better experience for someone within an organization to navigate through multiple apps?

If a single application exists, does it try to do too much, therefore complicating the purpose?

When you're designing the forms for the app, make sure that each form has a purpose that you can define in a single, simple sentence. Avoid the urge to have a single form that contains too many purposes, such as creating customers and customer contacts. Instead, consider creating multiple forms, each with a specific purpose.

Responsive design
Any mobile application or website that is considered mobile-optimized should adapt to the application in which it's viewed.

For example, a website such as Microsoft.com can be viewed in desktop or mobile view. The application or website adjusts its layout for the design in which it's viewed. The following example shows Microsoft.com in a desktop view and then a mobile-optimized view.

![image](https://github.com/adeleke123/Power-Platform/assets/51156057/c387611b-076d-4eea-8d58-175aea732034)

Simplistic user interface
Resist the urge to include too many fields and input controls on a form.

It might seem like a good idea to include all fields that people might want to use for a task, such as creating a customer, so that the canvas app is comprehensive. However, providing several extra controls that people will rarely use will create a cluttered interface and create more scrolling and "field hunting" to find the fields that they use most often. Instead, consider creating a succinct form and creating a new form for advanced field entry that people would use only on rare occasions.

If users must navigate to multiple screens, they might have a negative experience.

When buttons are needed, such as a Submit button, consider where to place the button in relation to where it's easiest for users to select.

Design with simplicity:

If too many buttons and fields are on a screen, users might select a button or field by accident.

Consider adding buffer space around fields and Submit buttons to allow for user error variance.

Intuitive navigation
A mobile-optimized app shouldn't have to come with a complex user manual. Instead, organize the tasks and business actions in a way that guides the user through their daily operations.

Determine the most logical way to organize the tasks for a user based on the previously defined purpose. Consider the following two design scenarios:

The mobile app is used to create sales orders 90 percent of the time and create new customers 20 percent of the time. As a result, the first navigation button should be to the sales order creation form, and the second navigation button should be to the customer creation form.

The mobile app is used for the business use case of finding new customers by creating their first order. As a result, the first navigation button should be to the customer form, and the second navigation button should be to the sales order creation form.

Users will always want an easier way to "return home" or go back to the main screen. Therefore, keep the following considerations in mind when creating return navigation:

Each form should include a simple way to return to the main screen to conduct another action.

Requiring a customer to return to a central point through multiple actions will result in a poor user experience.

If a user finishes a specific task and has no new tasks to complete, then that user should be returned automatically to the home location, where they can conduct their next actions.

Exclude external peripherals
Likely, users who are on a phone or tablet won't have a mouse and keyboard.

When designing the application's user interface, you should try to imagine yourself holding a specific device in your hand and interacting with the application to help you determine whether it's a good experience or not. For example, when a user enters field information, a keyboard will likely appear on the device, so you should determine whether that factor will impact the user's experience.

Include offline capabilities
A mobile application will traverse multiple locations. As a result, ask yourself the following questions to help determine when users might need offline capabilities:

Could this application be used in a location where the user might need to conduct an action without internet connectivity?

Because including offline capabilities in a canvas app can be complex, will the efforts to make the actions offline-capable worth the effort?

Are the actions that need to be conducted offline unavailable on the device, such as reading/writing data that's only available at a specific location?

Connectivity alerts
In a cloud-first solution, connectivity to the cloud is imperative. Most users will assume that they have connectivity to the internet when they access the canvas app.

Different forms and actions that have internet connectivity requirements should include a form verification. Before the user attempts to enter data, this form verification can alert the user that the mobile application is in offline mode and that the action isn't available. For example, if the action of creating a customer requires connectivity, then the application shouldn't allow a user to access the customer creation form and enter data when the mobile application is offline.

Alerting the user as soon as possible will help reduce potential data entry rework. You should consider including an alert indicator, such as a banner on the top of the screen indicating that the mobile application doesn't have connectivity.

Seamless setup
Seamless setup is vital to users who are adopting the app. Microsoft's deployment of Power Apps makes the deployment seamless, but configuration might be required in scenarios where you're connecting those apps to necessary data sources or user access.

When prompting the user to enter data that's required to run the application, such as a URL to an application or API, you should consider including tips for users to find that data. Assume that this time is the user's first for using the application and that they need guidance.

Additionally, you should consider including a comprehensive and direct description of the mobile application that tells users what app is being used.

Optimize for performance
Performance is more important for mobile applications than desktop applications. The limitations of multitasking with several tasks on a mobile phone make performance a significant factor. Desktop users can almost effortlessly navigate to another application while the canvas app does specific tasks.

When optimizing the app for performance, you should:

Consider the data sources that are being used and the complexity of the data that's being retrieved.

Evaluate the data connectors that are being used for the application.

Try to eliminate complex or unnecessary data sources.

Try to only retrieve the specific number of records that are required for a given action.



