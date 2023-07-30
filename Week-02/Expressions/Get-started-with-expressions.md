## Get started with expressions

To write an expression in Power Automate, select a field to open the Dynamic content menu and then select Expression as shown below.

![image](https://github.com/adeleke123/Power-Platform/assets/51156057/bd199d3b-ce97-40f8-8bde-130d26589785)

![image](https://github.com/adeleke123/Power-Platform/assets/51156057/6cd5d842-1222-4da3-885e-4259d3c4d60a)

![image](https://github.com/adeleke123/Power-Platform/assets/51156057/c61e98ce-cb43-408e-b1da-a8ffaf71302f)

This can be daunting. What does it want for the time zone? If you look in the pop-up, you'll see that it provides a link to the list of time zone values. This page provides you the string for the destinationTimeZone. With that information, we can now complete the expression.

`convertFromUtc('2020-09-01T12:00:00Z','Eastern Standard Time')`

Once the expression is completed, you can select OK to save your changes. Always be sure to select OK or UPDATE when editing an expression. If you select out of the inputs, you will lose your changes. Power Automate does not have AutoSave.

With your first expression complete, you can now select Test in the top right-hand corner. Then select Save & Test.

Once the test has completed, you should see the green bar that says "Your flow ran successfully." Expand the Compose action and you'll see that the OUTPUTS is your date time converted to the new time zone.

![image](https://github.com/adeleke123/Power-Platform/assets/51156057/91f3c56a-1e7e-4789-8f06-ff8ec422353a)
