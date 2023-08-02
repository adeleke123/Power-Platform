## Create recurring flows.

In this unit, you'll learn how to build prescheduled flows by using a trigger called recurrence. You'll build a flow for the Contoso marketing team that automatically pulls customer email addresses from a Microsoft Excel workbook on Microsoft OneDrive. You'll then set up the flow so that any new email addresses that anyone adds to the workbook are added to a MailChimp customer list once a day.

## Prerequisites
For this scenario, you’ll need to make an Excel file with a table that contains the following columns: ContactEmail, FirstName, and LastName. Save the Excel file in OneDrive for Business. You'll connect to this file in step 9.

![image](https://github.com/adeleke123/Power-Platform/assets/51156057/f6c07d68-b649-407c-92e1-301f533d2dc5)

## Create a scheduled flow
+ Sign in to Power Automate by using your organizational account.

+ Select My flows.

+ Select New, and then select Scheduled cloud flow.

By default you have the option to repeat every 1 minute, however, you have the option to change it and the options available are Minute, Week, Day, Hour and Second.

![image](https://github.com/adeleke123/Power-Platform/assets/51156057/fa0eeae4-e788-4dad-b08c-73ceac20fa3f)

![image](https://github.com/adeleke123/Power-Platform/assets/51156057/735d9707-c453-4d92-976e-f62ca5284859)

![image](https://github.com/adeleke123/Power-Platform/assets/51156057/67ef041c-4d50-4423-8a54-cc4c2c718f13)

![image](https://github.com/adeleke123/Power-Platform/assets/51156057/f5203100-7d38-4e95-8b6b-42b24d9ed456)

![image](https://github.com/adeleke123/Power-Platform/assets/51156057/a84b4113-676b-409a-8d78-9daf5fa86a7b)

And there you have it!

This flow will now run once a day. It will:

+ Get the new rows from the Excel worksheet

+ Grab the email address and name from each row

+ Enter the email address and name in the Contoso MailChimp mail list

+ Save you both time and money

![image](https://github.com/adeleke123/Power-Platform/assets/51156057/698a567e-75f7-45d7-ab75-518088185ee4)








