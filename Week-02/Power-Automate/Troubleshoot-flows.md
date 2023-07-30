## Troubleshoot flows

In this unit, you'll learn how to troubleshoot common issues that might occur while you run your flows.

## Identify the error
Before you can fix a flow, you must identify why it failed. You will get an email with a list of failures each week.

Select the Monitor and then Cloud flow activity on the left menu (or select the Activity tab in the mobile app), and then select your flow in the list that appears.

![image](https://github.com/adeleke123/Power-Platform/assets/51156057/468fc407-ea39-4ac0-8462-cc23a5155f72)

![image](https://github.com/adeleke123/Power-Platform/assets/51156057/e114279a-3ffe-4248-abfe-540fc2449c23)

## Authentication failures
In many cases, flows fail because of an authentication error. If this type of error occurs, the error message includes the word "Unauthorized," or an error code of 401 or 403 appears. You can usually fix authentication errors by updating the connection.

You can view the connections by opening up the flow details by selecting the flow from My Flows.
Scroll to the connection that you saw the "Unauthorized" error message for.
Next to the connection, select the Fix connection link in the message that states that the connection hasn't been authenticated.
Verify your credentials by following the instructions that appear. Then return to your flow-run failure, and select Resubmit.
The flow should now run as expected.

## Action configuration issues
Flows sometimes fail if a setting in one of the flow's actions doesn't work as expected. In this case, the error message includes the phrase "Bad request" or "Not found," or an error code 400 or 404 appears.

The error message should indicate how to fix the failure.

Select the Edit button, and then fix the issues inside the flow definition.
Save the updated flow, and then select Resubmit to try to run the flow again with the updated configuration.
## Temporary issues
If error code 500 or 502 appears, the failure is temporary or transient.

Select Resubmit to try to run the flow again.
Issues with your pricing plan
Sometimes your flows might behave unexpectedly because you aren't using the correct plan.

To view your plan, in Power Automate, select Learn. It will redirect you to the Microsoft Power Automate documentation page. Here select Learn Power Automate, and then select Pricing.

![image](https://github.com/adeleke123/Power-Platform/assets/51156057/967dc801-dfec-4d8f-ba85-be197492018e)

![image](https://github.com/adeleke123/Power-Platform/assets/51156057/5607ecbc-c183-4d5b-9de2-eb6541a2f39b)

## Some flows run more often than expected
Some flows might run more often than you expect. For example, you create a flow that sends you a push notification whenever your manager sends you an email. That flow must run every time you get an email from anyone, because the flow must check whether the email came from your manager. This action counts as a run.

## Other issues that are based on limits, and caveats
You might have issues that are based on other limits:

Each account can have up to:

600 flows.
50 custom connectors.
20 connections per application programming interface (API) and 100 connections total.
You can install a gateway only in the default environment.

Some external connectors, like Twitter, implement connection throttling to control the quality of service. Your flows might fail when throttling is in effect. If your flows are failing, review the details of the run that failed in the flow's run history.

