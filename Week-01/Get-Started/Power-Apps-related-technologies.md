## Power Apps related technologies

#### Data sources, connections, and gateways

In Power Apps, most canvas apps use external information that is stored in Data Sources. A common example is a table in an Excel file that is stored in OneDrive for Business or SharePoint. Apps access these data sources by using connections. Some connections allow Power Apps to read and write stored data. In Power Apps, you can add many data sources to your apps through built-in or custom connectors. Some of the most popular data sources are shown in the following figure.

![image](https://github.com/adeleke123/Power-Platform/assets/51156057/1a23ef6e-8658-4686-9630-92477411e783)

Many data sources are cloud services, like Salesforce. Even Twitter can be a data source if, for example, you're tracking your company's hashtags. Connectors might not seem like the most exciting part of app development; however, they're essential when you work with data that you, your colleagues, and your customers care about. When an app shows up with your data source for the first time, you might suddenly find that they are, in fact, exciting.

For data that's stored on-premises instead of in the cloud, you can use a gateway to provide a reliable connection between Power Apps and your data source. The gateway sits on an on-premises computer and communicates with Power Apps.

An advantage of building your business apps in Power Apps is being able to connect to many data sources in a single app. With the connectors in Power Apps, you can connect to where your data lives. To learn more about data sources in Power Apps, refer to the Working With Data learning path.

![image](https://github.com/adeleke123/Power-Platform/assets/51156057/afbe0a06-5a55-436c-b0b4-3c0c03dfc53b)

### Microsoft Dataverse

An important data source option to explore further is the Dataverse. Dataverse lets you store and manage data that's used by business applications. Data within Dataverse is stored within a set of tables. A table is a set of records that are used to store data, similar to how a table stores data within a database. Dataverse includes a base set of standard tables that cover typical scenarios, but you can also create custom tables that are specific to your organization and then populate them with data by using Power Query. App makers can then use Power Apps to build rich applications by using this data.

![image](https://github.com/adeleke123/Power-Platform/assets/51156057/0e6522e9-dfa0-466e-9f8a-d9f850f875c7)

### Reasons to use Dataverse
Standard and custom tables within Dataverse provide a cloud-based storage option for your data. Tables let you create a business-focused definition of your organization's data for use within apps. If you're unsure if tables are your best option, consider the following benefits:

+ `Simple to manage` - Both the metadata and data are stored in the cloud. You don't need to worry about the details of how they're stored.
+ `Helps to secure data` - Data is stored so that users can see it only if you grant them access. Role-based security allows you to control access to tables for different users within your organization.
+ `Access your Dynamics 365 Data` - Data from your Dynamics 365 applications is also stored within the Dataverse, which allows you to quickly build apps that use your Dynamics 365 data and extend your apps by using Power Apps.
+ `Rich metadata` - Data types and relationships are used directly within Power Apps.
+ `Logic and validation` - Define calculated columns, business rules, workflows, and business process flows to ensure data quality and drive business processes.
+ `Productivity tools` - Tables are available within the add-ins for Microsoft Excel to increase productivity and ensure data accessibility.
