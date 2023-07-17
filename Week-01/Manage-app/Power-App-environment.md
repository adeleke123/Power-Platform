## Exercise - Understand environments in Power Apps

An environment is a container for apps and other resources, such as data connections and flows from Power Automate. It's a way to group items based on business requirements.

![image](https://github.com/adeleke123/Power-Platform/assets/51156057/12f3deba-0010-4fef-928b-4c3e808b34a5)

If you've followed along with this module, you've already been working in make.powerapps.com. Therefore, you've been working in a specific environment the whole time. In the upper-right corner of the home page, you can view your current environment.


![image](https://github.com/adeleke123/Power-Platform/assets/51156057/d1cfff9f-3e51-4eac-9ea9-e6eea151b064)


## Reasons to use environments
Reasons to create environments beyond the default one include:

+ Separate app development by department - In a large organization, each department can work in a different environment. That way, department employees see only apps and company data that are appropriate to their needs.

+ Support application lifecycle management (ALM) - Separate environments let you separate apps that are in development stages from ones that have already been shared. Alternatively, you might want to use a trial environment so that you can receive feedback from employees before publishing the final app. For some organizations, showing apps before they're completely developed and published can present security concerns.

+ Manage data access - Each environment can have its own source of business data, called a database for Microsoft Dataverse. Other data connections are specific to an environment and can't be shared across environments.

Create an environment
Only an admin can create environments. If you aren't an admin, this information can still be helpful when you talk to your admin about setting up environments.

On the make.powerapps.com home page, select the gear icon near the upper-right corner and then select Admin center.

You can also go directly to https://admin.powerplatform.microsoft.com

In Microsoft Power Platform admin center, select + New.

In the New environment dialog box, enter a name for the environment and then select a region and an environment type.

To the left of Create a database for this environment, select the toggle to Yes.

Select Next.

Select the currency and language for the data that is stored in the database. You can't change the currency or language after the database is created.

Select Save.

It might take several minutes to create the database on Dataverse. After the database is created, the new environment appears in the list of environments on the Environments page.

You now have a new environment to work in. If you go back to make.powerapps.com, you'll see it in the environments list.

Manage access to an environment
By default, you can access an environment in one of two ways:

System admin - A system admin has full permissions to create and manage environments.

Environment maker - An environment maker can view all apps in that environment, create apps, and work with Dataverse (other permissions apply).

Environment admins can create other security roles as needed. They can also add and assign users to these roles.

Start by going to https://admin.powerplatform.microsoft.com

On the left pane, Environments should be selected by default, if it isn't, select Environments.

Select the test environment that you created, and then select Settings at the top.

Select the Users + permissions dropdown and select Users.

Select Add user at the top and add the user by entering the email address of the user in your organization and then selecting Add. Wait a few minutes for the user to be added.

To manage the roles and information of a user, select the user’s Name. A new tab opens with the Dynamics 365 view of that user.

Select Manage Roles on the top bar.

In the Manage User Roles box, select the role(s) for the user. In this example, assign the user to the Environment Maker role.

Select OK.

The changes are then saved, so you can close the Dynamics 365 tab in your browser when done.

