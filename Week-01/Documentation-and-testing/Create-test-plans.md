## Create test plans

As part of your Canvas App deployment, the next step is to begin testing it. This unit will help you understand the basics of how you should carry out your testing. Let's consider three types of testing to include in your plan.

## Types of tests
+ Unit tests
A Unit test is the smallest component of testing. It's used to check whether a specific function or feature of your app is working.

## End-to-end tests
End-to-end tests are used to check whether the overall solution runs correctly. They're important because even if all unit tests function correctly, the integration between unit tests can potentially fail. You would perform these types of tests by following a test scenario that's close to the use case of the actual business process.

## User acceptance tests
A User acceptance test (UAT) is one that's done by the user of the app instead of the maker. This test ensures that what has been built by the makers matches the requirements initially requested by the user.

## To get the most out of your UATs, here are some tips:

+ Test with the actual users.

+ Try to choose users with diversity in terms of IT skill levels. This way, you can get various types of feedback.

+ Don't give the user instructions; see whether they can understand the app intuitively.

+ Observe how users navigate the app without assistance and see where you can improve the design.

+ When a user is stuck on a screen, ask them to explain what their expectation was.

+ Try out different devices to make sure the test cases behave the same, regardless of the platform.

+ Test offline capabilities - ideally, test the app in the user's actual environment or location if the app uses offline capabilities.

+ Ask your test users to try to "break" your app, such as by entering unusual characters in text fields.

+ Users will typically test the "happy path" (the path a user takes when everything is going perfectly). Ask them to also test scenarios such as canceling an expense report instead of submitting it, or denying an expense report instead of approving it.

Your users might not be familiar with software testing, so let them know what kind of feedback you're looking for. It's often helpful to provide a template for "bugs" to make sure testers explain:

+ Exactly what they were doing
+ What happened
+ What they expected to happen instead
+ Any relevant information about their testing environment such as device type and browser.
It's natural and acceptable for the user to request changes to the specifications or ask for more features. These requests should be recorded in a feature list like the one described in Prioritizing features and requests so you can prioritize and incorporate them into the app.

## Creating test cases and scenarios
In planning for testing, you should consider the important scenarios that you may have identified in the planning and design phases of your Power Apps project.

Your first step is to write the unit tests. You'll want to break down the tests to each feature or function. The test cases for unit tests should be listed in a manner like this table:

![image](https://github.com/adeleke123/Power-Platform/assets/51156057/43e86dfa-cb8a-4539-82a8-8e7e4bef35b0)

In summary, a good plan will help your testing go smoothly. Your goal is to create a test plan that describes the intention and scope of testing, guides the technical review process and supports a smooth rollout of functionality. Your test plan development should precede user acceptance testing and have a means for tracking changes needed before rollout.

