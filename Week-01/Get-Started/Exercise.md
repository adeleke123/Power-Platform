## Exercise - Create your first app in Power Apps

In this unit, you'll generate a mobile app where the data source is a Microsoft Excel workbook that's stored in Microsoft OneDrive for Business. This Excel workbook lists a company's inventory of flooring samples with pictures and prices.

Keep in mind that you can use data from many other sources, including Microsoft SharePoint, cloud services like Salesforce, and on-premises sources like Microsoft SQL Server.

### Connect to a data source

To connect to a data source, use the following procedure:

+ Download the Flooring Estimates workbook and save it to OneDrive for Business.

+ Go to https://make.powerapps.com and sign in with your organizational account.

+ On the Home or Create screen, select Excel. After a few moments, you'll navigate to the Connections screen. If your connection doesn't immediately show, select Refresh.

+ After a few moments, you should see your existing connections. Select (or add as a connection) OneDrive for Business.

+ Generated apps are always based on a single list or table, but you can add more data to the app later. The next three steps explain how to connect to the Excel workbook.

+ Still in your Connections screen, you should now see a list of Excel files under the header Choose an Excel file including the FlooringEstimates.xlsx. Select the FlooringEstimates file.
![image](https://github.com/adeleke123/Power-Platform/assets/51156057/f6ff5c2f-ba1c-4718-8e42-de523a3ef40f)

+ Under Choose a table, select the FlooringEstimates table.

+ Select Connect on the bottom right.

Power Apps generates the app by inspecting your data and matching it with Power Apps capabilities so that you get a working app as a starting point.

### Explore the generated app
Your new three-screen app now opens in Power Apps Studio.

The following figure shows the main development window for Power Apps Studio, which you'll learn more about in later units.

![image](https://github.com/adeleke123/Power-Platform/assets/51156057/4656a9af-30fe-4ac8-a255-01bcbd70ab7d)

Put your app in Preview (or Play) mode by selecting the "play" button in the upper-right corner of the screen (or by selecting F5) to practice using the app. Notice that your app includes all the data from the table and provides a good default experience.

All apps that are generated from data have the same set of screens that you can view from the Screens pane:

+ `Browse screen` - This screen appears by default. In it, you can browse, sort, filter, and refresh the data from the data source. In the browse screen, you can add items to the data source by selecting the plus sign (+).
+ `Detail screen` - The detail screen shows all information about a single item. In this screen, you can open an item to edit or delete it.
+ `Edit screen` - In this screen, you can edit an existing item or create a new one.
To make your app visible on the phone, it needs to be saved. Select the drop-down to the right of the Save icon at the top right of the screen, and select Save as. Replace the current title "App" with Flooring-estimates app, and then select Save. You can now open the app on your phone.

### Install the app on your device
To see how the app runs on mobile, install the Power Apps Mobile app on your phone. When building an app, you should test it in the same form factor as your users.

+ Download Power Apps Mobile from the app store for the platform that you want to use.

+ Sign in by using your username and password.

+ On your phone or tablet, run the Flooring-estimates app in Power Apps Mobile. If you don't want to install the app, you can run it in a browser.

+ If you don't see the Flooring-estimates app, then in your Power Apps Mobile app, select the user account menu and select All apps. Enter "Flooring" in the search field at the top of the screen.


