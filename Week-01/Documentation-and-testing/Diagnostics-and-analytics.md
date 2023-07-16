## Diagnostics and analytics

Designing for performance is an important part of the process and so is performance testing. When conducting performance testing, try to replicate in your tests where the volume of data is close to your production system. That will give you a good understanding of app performance in general and for the areas to optimize.

So how can you diagnose what's going on with your app and analyze your tests? In this unit, we'll do a more thorough introduction to some tools that are available to help you do these things.

## Monitor
## Overview
Monitor, which we introduced previously, is a tool that offers makers the ability to view a stream of events from a user's session to diagnose and troubleshoot problems. Makers of canvas apps can use Monitor either to view events while building a new app in Power Apps Studio or to monitor published apps during runtime.

## Benefits
Monitor can help you diagnose and troubleshoot problems faster and build more reliable apps. It provides a deep view of your app by logging all the key activities that occur in the app as it runs. Monitor also provides a better understanding of how the events and formulas contained in your app work, so you can improve performance and identify any errors or problems.

## Debugging an app
The key to debugging a problem is to gain a better understanding of what your app does, and how it does it. Sometimes it's difficult to isolate a problem by just looking at the app formulas, or even by reviewing runtime errors. Watching the events as they occur in your app can help you understand the order of events and how your app is performing, to spot errors and diagnose problems faster.

## Monitor dashboard
The Monitor dashboard enables you to review properties for each app event. You'll get an idea of what happens when you select a control, the duration of the process, and the outcome of the operation.

Here's an image of what the Monitor dashboard looks like, and after the image is a summary of what information each column in the dashboard contains.

![image](https://github.com/adeleke123/Power-Platform/assets/51156057/4b69cb6c-2876-4ab9-85df-7efcc501a76e)

Monitor properties panel
The Properties panel is available for a selected operation. To view the panel, select Properties from the side rail on the right. The Properties panel has tabs portraying details about the event. Every event will have a Details and Formula tab, and if an event triggers an HTTP request/response, you'll also see tabs for Request and Response. This image depicts the Details tab for a SortByColumns event:

![image](https://github.com/adeleke123/Power-Platform/assets/51156057/1777c603-8dd6-46b2-a365-496f5f32f269)

## Starting Monitor
You can activate Monitor in two ways. When you're editing a canvas app, you can open Advanced tools, and then select Monitor.

![image](https://github.com/adeleke123/Power-Platform/assets/51156057/ef9b4ee2-a5b2-435d-ad07-ad9f06c5c1fb)

Another way to open it is by going to your Apps from the Maker portal, selecting any app, and then selecting Monitor from the header ribbon.

![image](https://github.com/adeleke123/Power-Platform/assets/51156057/2aa9c3a1-8c10-4b75-b949-3a4e21cdf067)

![image](https://github.com/adeleke123/Power-Platform/assets/51156057/b6ec8bf9-8a93-493d-ad01-1620a61b97d3)

![image](https://github.com/adeleke123/Power-Platform/assets/51156057/8215b8c2-1913-4526-88e1-22fd0f68fc04)


## Introducing Power Apps analytics
To help you analyze your app, Microsoft has provided Power Apps analytics, a series of reports providing a view into environment level usage, errors, service performance, and change management services to users. These reports are available for your canvas apps.

If you're an environmental admin, Power Platform admin or Microsoft 365 Global admin, then you'll have access to these reports. You can access them by signing into the Power Platform admin center and select Analytics > Power Apps. Reports will appear in a menu bar at the top of the page. We'll cover the different reports available next.

![image](https://github.com/adeleke123/Power-Platform/assets/51156057/424b636e-c37c-4dc2-a41f-2b29a958405d)

## Available reports
The Usage report is shown by default when logging into the admin center. It provides total app launches and daily active users across all apps in the environment. Admins can filter the view with attributes like device platform, player version, country/region, state, and city.

![image](https://github.com/adeleke123/Power-Platform/assets/51156057/169e28e3-e93e-4cce-9f94-cdb13482bf7a)

![image](https://github.com/adeleke123/Power-Platform/assets/51156057/641f9745-2fee-4984-af94-a5605e3f147f)

![image](https://github.com/adeleke123/Power-Platform/assets/51156057/19de5ada-75c8-444d-b0cc-60282dc2619e)

![image](https://github.com/adeleke123/Power-Platform/assets/51156057/b5caedca-0302-431b-bf43-6ebc8b94ea26)

![image](https://github.com/adeleke123/Power-Platform/assets/51156057/9e7a3b1e-569b-4205-85fb-053aa663a36c)

![image](https://github.com/adeleke123/Power-Platform/assets/51156057/72324ee9-21dc-4b60-90e9-9bc2dd7aa2d1)


It's possible to download reports and change environments within the app. Refer to Power Apps analytics to learn more.




