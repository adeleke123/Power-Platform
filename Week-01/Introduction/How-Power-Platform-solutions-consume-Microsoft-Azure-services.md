## Describe how Power Platform solutions consume Microsoft Azure services

The Azure cloud platform consists of hundreds of products and cloud services designed to help you bring new solutions to life to solve today's and future challenges. These services range from data storage services to virtual machines, to artificial intelligence services. Microsoft Azure service provides you with the opportunity to build, run, and manage applications across multiple clouds, on-premises, and at the edge, with the tools and frameworks of your choice.

Power Platform and Azure services are a perfect complement for each other, and the possibilities for using them together are endless. Azure services can be used with Power Platform to help modernize legacy systems, automate processes, and create advanced analytical solutions.

Let’s look at an example of how an organization might use Azure and Power Platform.

The example demonstrates how you can deploy portals to automate manual or paper-based processes and surface a rich user experience. Employ Azure API management and Azure Functions to connect custom APIs, which tap into your legacy systems. By using Azure-managed databases and a low-code approach to automate tasks, you can lower the overall solution costs. You can quickly build apps that are real-time, resilient, and scalable.

![image](https://github.com/adeleke123/Power-Platform/assets/51156057/127447e2-7321-426d-9d8b-f7d06606a5cf)


#### The data flows through the solution as follows:

+ The airline system communicates with a custom API hosted in [Azure API Management.](https://learn.microsoft.com/en-us/azure/api-management/)

+ A custom API coordinator receives notifications and handles incoming messages from the airline system, assigning flights to Microsoft Teams channels and sending them to [Power Apps.](https://learn.microsoft.com/en-us/power-apps/)

When a user selects a flight to monitor, or when the system assigns the user to a flight, the system queues a Graph API call in an Azure Storage Account queue for further processing.

[Azure Functions](https://learn.microsoft.com/en-us/azure/azure-functions/) runs the Graph API calls based on the incoming messages in the storage queue, sending notifications to Teams, and also streams all events to an [Azure Event Hubs](https://learn.microsoft.com/en-us/azure/event-hubs/) for further analytics.

The airline's notification system is managed by a custom bot messaging service that employs [Azure Bot Service.](https://learn.microsoft.com/en-us/azure/bot-service/?view=azure-bot-service-4.0)

Custom bots send flight updates to users in Teams.

An [Azure Data Lake](https://learn.microsoft.com/en-us/azure/storage/blobs/data-lake-storage-introduction) storage offers long-term retention and micro-batch processing of events from Event Hubs, ultimately generating insightful reports with Power BI.


