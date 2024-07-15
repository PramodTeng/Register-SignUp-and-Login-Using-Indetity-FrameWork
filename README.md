How this works:

Step1:

Add Identity To Our Project.(Right Click on the project, Go to Add, Select New Scaffolded item and Click on identity.)

* Add Layout Page(Master Page)
* Select Features you want to add in Identity.
* Create a Data Context Class which is used to communicate with our database.
* Create a user Class.

After Adding Identity there is a folder called "Areas" appears.


Step 2:

* Add Register/Login Links in the Navbar.  
* we have to call a "_LoginPartial.cshtml" partial view in our Layout Page by using partial tag. (<partial name = "_LoginPartial" />)
* "_LoginPartial.cshtml" partial view is located in Views/Shared folder, and that is added by identity.
* Dont forget to add app.MapRazorPages(); in the program.cs for RazerPage view.

Step 3:
* Add Some Properties in Application User Class.
* Register these properties OR Configure in ApplicationDbContext Class.

Step 4:

* Now Add Connection String inside appsettings.json
* Add-Migtration
* Update-Database

Step 5:
* After updating the database add the properties that is defined in the ApplicationUser Class (i.e firstname and lastname)
*  Also modify the  InputModel class that binds this properties.

Run the application and test the program.

If you want to make the  SignIn.RequireConfirmedAccount false , change it from the Program.cs




