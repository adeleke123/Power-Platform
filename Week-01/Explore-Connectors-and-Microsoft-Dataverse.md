### Explore connectors and Microsoft Dataverse

Typically, when organizations are building business solutions, how the solution will work and perform can be impacted by several factors. Two of those areas are connecting to data sources and managing business data. Power Platform includes two tools that make these areas easier. They are data connectors and Microsoft Dataverse. Data connecters make it easy to connect to data across different services. Microsoft Dataverse is a business database that not only stores business data, but also includes other built-in features such as security and more.

_Let’s take a moment and examine each of these elements a little more closely._

### Connectors

Creating solutions that span multiple services can create challenges. One of those challenges is ensuring that you can perform the necessary operations in all systems. The challenge is that you need to be access the service with a valid account, but that the account needs to be able to perform the necessary actions across all services. Let’s look at the following document processing example.

A building management uses vendors to perform services at their buildings, such as cleaning properties after tenants leave and providing landscaping services at their properties. After the jobs are completed, vendors send invoices to the building management company. The building management company may want to automate processing invoices from vendors.

### Currently the process is as follows:

+ Invoices are received as email attachments. The management company uses Microsoft Exchange for processing emails.

+ These attachments are downloaded and stored in Microsoft SharePoint.

+ Each invoice is sent to a specific person for approval. Approval is made in Microsoft Teams.

+ Once approved, the invoices are entered into the company’s ERP system. The management company uses Oracle.

+ Once entered, a confirmation email with the invoice number must be sent back to the vendor.

Automating a process like this requires interaction with multiple services. There are likely different accounts being used with each service, and different data operation that are being executed. In this example, we would be working with at least four different services.

+ `Office 365 Outlook:` First, you would need to monitor a specific Microsoft Exchange mailbox.

+ `Microsoft SharePoint:` Attachments are downloaded and saved to a specific folder in Microsoft SharePoint.

+ `Microsoft Teams:` Invoice approval requests are sent to managers in Microsoft Teams, where they can either approve or deny the request.

+ `Oracle:` Once approved, the new invoice is created in Oracle. Details of the invoice are stored so they can be used alter.

+ `Office 365 Outlook:` A confirmation email is sent using a dedicated mailbox to the company that submitted the invoice.

With Power Platform, data connectors make working with different data sources easier. They act as the bridge between data sources and your app or workflow. Power Platform has more than 900 connectors available to various data sources. Connectors also include a series of actions that simplify the process of working with those data sources. For example, the Office 365 Outlook connector has prebuilt actions for working with mailboxes, such as downloading attachments, and sending emails, managing events, and more. When using a connector, you just need to provide some basic details about the action you want to complete. Data connectors are used throughout Power Platform. For example, in Power Apps, they are used to connect apps to data. A company might create an order fulfillment application for their employees who work in the field. Data connectors would be used to connect the app to data sources like an SQL database or Microsoft Dataverse. In Power Automate, data connectors can be used to connect to data sources that are used as either triggers or actions.

### Microsoft Dataverse

Microsoft Dataverse allows organizations to securely store and manage data used by your business applications. Dataverse data is stored in tables. A table is a set of rows and columns. Each column in a table stores specific type of data such as names, locations, ages, dates, salaries, and so on. In addition to data storage, Dataverse also has other elements that help with securing data, data validation, and productivity.

Each Dataverse instance includes a base set of standard tables that cover typical business scenarios such as accounts, contacts, and activities. This base set of tables reduces the amount of time that it takes for organizations to start building solutions since there are already standard business tables available. Additionally, organizations can also create custom tables specific to their needs and populate them with data.

### For example:

+ A real estate company might create tables to store the properties they sell, represent open houses, or store showings.

+ A financial company might add tables to represent loan applications or bank accounts.

+ An auto repair company might add tables to represent the parts they sell or the services they provide.

Once the tables are created, application makers can use tools like Power Apps to build rich business applications that use this data. For example, a real estate company might create a property management application for their agents working in the field. The app would provide agents with access to the properties stored in Dataverse.

### Using Dataverse provides these benefits:

+ `Easy to manage:` Both the metadata and data are stored in the cloud.

+ `Easy to secure:` Data is securely stored so users can only access what they need to. Role-based security allows you to control access to tables for different users within your organization.

+ `Rich metadata:` Data types and relationships are used directly within Power Apps.

+ `Logic and validation:` Define calculated columns, business rules, workflows, and business process flows to ensure data quality and drive business processes.

+ `Productivity tools:` Tables are available within the add-ins for Microsoft Excel to increase productivity and ensure data accessibility.

Many solutions built on Power Platform use both Dataverse and connectors heavily. Dataverse acts as the primary business data storage mechanism, and connectors are used in the different apps and automations that are connecting to different data services.

Now that we have introduced you to some of the primary elements of Power Platform, let’s see how it can be used with other services.
