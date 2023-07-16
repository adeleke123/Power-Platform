## Performance optimization

To determine how to optimize the performance of your app, let's first cover what happens with your app when it starts. Then we can discuss some common sources of slow performance.

## App execution phases and data call flow
Before your user even begins to interact with your app, there are some phases of execution that the app goes through first. After that, your app conducts a data call flow that varies depending on the data source.

## Execution phases in canvas apps
A canvas app progresses through the following phases of execution before showing the interface to a user:

Authenticate the user: this execution phase prompts first-time users to sign in with their credentials for the app's connection. Depending on the organization's security policies, the same user may be prompted again whenever that person reopens the app.
Get metadata: retrieves metadata such as the version of the Power Apps platform on which the app runs and the sources from which it must retrieve data.
Initialize the app: performs the tasks specified in the app OnStart property.
Render the screens: renders the first screen of the app including the controls and data portrayed on the first screen. Similarly, the app goes through the same process to render any subsequent screens opened by the user.
Data call flows in canvas apps
Data calls from canvas apps use OData protocol to send and receive data. In many cases, the data call goes from the app to Azure API management, from API management, to the data source, and then it must travel back to the app in reverse order. Also, if there's an on-premises data source (such as a SQL server), then the call must also proceed through an on-premises data gateway.

All of these call flow gates can cause performance considerations and potential opportunities for optimization. However, there's a significant difference in the data call if your app uses Microsoft Dataverse as the data source. When your data call goes to a Dataverse source, the OData request goes directly to Dataverse, without going through Azure API Management, connectors, or data gateways. In other words, there are fewer gates to get through when you're using Dataverse.

Common sources of slow performance for canvas apps
Now that you have a basic understanding of execution phases and flow of data calls, let's cover some of the most common sources of poor performance in canvas apps.

## App design
App design is a broad area because there are many ways that an app can be designed, however, some aspects that can certainly affect app performance include:

The app is client-heavy meaning that it gets large sets of data into data collections initially and then uses the data within multiple screens over client-heavy operations like JSON, Sort, AddColumns and GroupBy.
The app has a long formula in OnStart where it potentially triggers many unnecessary data calls in screens, and these data calls return large data records.
To review the app design as a possible source of slow app performance, monitor the app by using Monitor. Check which data calls are taking a long time, and how many data calls trigger such behavior in the app.

Also, try to balance the workload between the client and server, delegating the workload to the server is recommended when possible. From the perspective of client memory consumption, it's important to make the client app lightweight.

## Bottleneck in the data source
There are many possible causes of bottlenecks in the data source. But the most common is that tables in the data source are at the center of activity when many transactional or non-transactional queries are directed to the same table or record from different users.

OData calls might slow down if:

The back-end machine hosting the data source is low on resources.
The back-end SQL instance has blockings, deadlocks, or resource contention.
The on-premises data gateway is unhealthy.
When these problems occur, tune the back-end data source to avoid slowing the app's performance.

Client browsers, devices, and locations
Canvas apps can be used on different devices, browsers, and locations with varying network conditions. Encourage your users to use modern, updated and supported browsers.

Geographical location of the on-premises data gateway and environment
Users can access canvas apps globally. However, we recommend that you locate the data source near your largest user base. For example, when your app accesses your on-premises data source, the location of on-premises data gateway should be close to the data source to minimize any extra overhead between the data gateway and the data source.

Temporary throttling of high-volume requests at the back end
Depending on how you design a canvas app, it can generate many data calls within a short time. When data calls exceed a connector's throttling limits, the app is subject to a temporary throttle. So choosing the right data source and connector is important from many perspectives, and it's important to understand connector-specific limits. You can check the documentation on connectors to learn about any limitations they may have.

Debug published app setting enabled
Enabling the setting Debug Published app will cause your apps to perform more slowly. You can republish your app with this setting disabled when you determine that you no longer need to view source expressions when debugging your published app.

To summarize, we've now discussed what happens when a user begins using the app for the execution phases and the data call flow. We've also covered some of the common ways that your app performance can be degraded. Though we won't cover any more in this unit, you can learn about practical tips and best practices to improve performance of canvas apps, and considerations for optimized performance in Power Apps.


