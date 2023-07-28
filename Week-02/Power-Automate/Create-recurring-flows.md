## Create recurring flows

In this unit, you'll learn how to build prescheduled flows by using a trigger called recurrence. You'll build a flow for the Contoso marketing team that automatically pulls customer email addresses from a Microsoft Excel workbook on Microsoft OneDrive. You'll then set up the flow so that any new email addresses that anyone adds to the workbook are added to a MailChimp customer list once a day.

## Prerequisites
For this scenario, you’ll need to make an Excel file with a table that contains the following columns: ContactEmail, FirstName, and LastName. Save the Excel file in OneDrive for Business. You'll connect to this file in step 9.

![image](https://github.com/adeleke123/Power-Platform/assets/51156057/f6c07d68-b649-407c-92e1-301f533d2dc5)

## Create a scheduled flow
+ Sign in to Power Automate by using your organizational account.

+ Select My flows.

+ Select New, and then select Scheduled cloud flow.

By default you have the option to repeat every 1 minute, however, you have the option to change it and the options available are Minute, Week, Day, Hour and Second.
