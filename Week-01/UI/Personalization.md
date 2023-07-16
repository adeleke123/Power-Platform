Personalize

In Power Apps, you can show information about the current user with the User() function. This includes the full name, email address, and the picture that's associated with the user who's signed into a canvas app. It matches the "Account" information that is displayed in the Power Apps players and studio, which can be found outside of any authored apps. This may not match the current user's information in Office 365 or other services.

The User function returns a record of information about the current user:

![image](https://github.com/adeleke123/Power-Platform/assets/51156057/0b4047c2-8b7a-425d-9358-0d0dd35719c1)

Set the Image property of the Image control to this value to display the image in the app. Here’s an example of how to add a user's profile picture, email, and name to your app.

1. On the ribbon, select + Insert, expand Media, and then select Image.

2. Set the Image property to this formula: User().Image

3. On the ribbon, select + Insert, and then under Popular section select Text label:

4. Set the Text property to this formula: User().FullName

5. Move the label so it's below the image control.

6. Add another label, and set its Text property to this formula: User().Email

7. Move the label so it's below the first label:

![image](https://github.com/adeleke123/Power-Platform/assets/51156057/13c9267d-dd3c-4035-a42f-cf53ab707b3d)
