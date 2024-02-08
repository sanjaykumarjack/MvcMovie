LAB-1
Student Name- Sanjay kumar punyamanthula
student Id-0851634
2024-02-06

Task1: Create a web app using ASP.NET Core MVC and Visual Studio

CHALLENGES :

No challenges found because VS downloaded and configured as per the steps

SOLLUTIONS:

I download and install Visual Studio 2022 Preview with the ASP.NET and web development
workload in order to install and setup the necessary tools and frameworks. I installed the target framework 
for ASP.NET Core 8.0, which is.NET 8.0 (Long Term Support).
I have to launch Visual Studio and choose build a new project in order to build a new project with the ASP.NET 
Core Web App (Model-View-Controller) template. ASP.NET Core Web App (Model-View-Controller) should be selected in
the Create a new project window.
Ctrl+F5 to launch the web application without the debugger in order to run and test it locally. 
A dialog box to trust the IIS Express SSL certificate will appear in Visual Studio. If you are confident with the 
certificate, click Yes. Visual Studio will then launch the application and launch the default browser.


Task2:
Add a controller to an ASP.NET Core MVC application.

CHALLENGES:

How can I create a controller template using the scaffolding (tools) feature?
How can the routing logic that associates the URL with the controller action be specified?

Observation : 

Adding a controller to an ASP.NET Core MVC app involves creating a class
inheriting from Controller in the Controllers folder. Within this class, actions representing
various routes and HTTP methods are defined, each adorned with attributes like [HttpGet], [HttpPost].
A cshtml file  is created in the Views folder as HelloWorldController and arranged according to the controller name in order
to add a view to an ASP.NET Core MVC application. The view may create content dynamically by combining 
Razor syntax with HTML markup. 

STEP-3

CHALLENGES:

OBSERVATION:

Replace the content of the Views/Shared/_Layout.cshtml file with the following markup.
Controller actions are invoked in response to an incoming URL request. A controller class is where the code is written
that handles the incoming browser requests. The controller retrieves data from a data source and decides what type of
response to send back to the browser.

LAB-2

Student Name- Sanjay kumar punyamanthula
student Id-0851634
2024-02-06

TASK-1- Create a model for an ASP.net Core MVC application.
1) Included a class for data models: To represent the application's data model, a Movie class
is created in the Models folder, and a MovieContext class—which is derived from DbContext—is generated 
in the Data folder. This class contains a DbSet for the Movie model and represents the database context.
2) From the tools menu, choose NuGet Package Manager and the Package Manager Console to start the migration.
3) Launched the application, clicked the Movie App link, and looked at the registration and context class
that were generated in the database.
4) Looked at the migration file Migration Initialcreate.cs. 

Task 2: Use an ASP.NET Core MVC application's database.
1) Opened the SQL Server Object and examined the database using the view menu option 
2) In the models folder, I made a new class called SeedData, changed the code, and added a new list of movies.
3) The code could see the list of movies seeded when it was executed since the seed initializer had been included and had altered the contents of the program.cs class.


OBSERVATION:

A comprehensive how-to manual for building a basic web application that facilitates the creation, reading, updating, and deleting of data from a database.
In order to handle HTTP requests, I learned how to design and use controller methods.
Views: Recognized how to construct and apply views to provide data to the user.
Examined the use of model binding to translate HTTP requests into parameters for action methods.
Tag helpers: I gained knowledge on how to create HTML components in Razor views using tag helpers.




LAB-3

Student Name - Sanjay kumar punyamanthula
student Id-0851634
2024-02-07

Task 1: Include search in an ASP.NET Core MVC application
Changes to the controller:
Included search capabilities in the action methods of the controller that manage data display.
Data was extracted and filtered according to the search parameters.
Added a search form and showed the search results to the corresponding views. 
Designed and implemented an HTML form to collect user input for the purpose of doing a search.
To manage the submission of the form, an action method was defined in the controller. Taken the 
search query out of the form and applied it to the data filter.
modified the data access logic to incorporate the search feature and implemented the search logic.
evaluated the returned results after filtering the data according to the search query.
Confirmed

OBSERVATION:

An ASP.NET Core MVC application needed to have its model and data context classes updated, as well as 
its views and controllers updated to accommodate the new field. The addition of a new field should be
carefully considered and made sure to be pertinent and essential to the operation of the app. 
In order to make sure that the app is functioning as intended, it is also crucial to thoroughly test it after 
adding a new field.
This method helps to create an interface that is more interesting and easy to use. 
A new field was also added to the ASP.NET Core MVC application, which meant that the model
needed to be created, the database schema needed to be updated, the views and controllers needed to be adjusted,
and the data in the new field needed to be properly validated and handled. The key goal was to retain a high degree 
of user interaction while integrating the new feature within the application's current structure.

step-9

launched Visual Studio and the ASP.NET Core MVC application: The Model Class was navigated to:
Determine which model class the data entity that needs validation belongs to, then open it.
Utilize Annotations in Data to Verify To specify validation guidelines for the properties, 
utilize data annotations, or attributes, inside the model class. For example, utilize [StringLength] 
for the maximum length, [Required] for fields that must be filled out, or create custom annotations for certain needs.


Observation:
ASP.NET Core MVC enables developers to create custom validation logic, supports client-side and server-side validation,
and provides users with instant feedback. This gives users quick feedback on their input, which improves the user
experience. In accordance with user choices, programs can show error messages in many languages thanks to the system's
support for error message localization. This improves user experience and enables more seamless integration with other systems.
Quick Responses to Users: By adding validation, the user experience is improved as users receive quick feedback on theirinput.
I could become more knowledgeable about server-side and client-side validation. Validation can be done both client-side 
and server-side with ASP.NET Core MVC. Client-side validation is mainly managed via data annotations, whereas server-side validation
makes sure that the data is intact on the server.
In addition to normal annotations, custom validation logic enables developers to apply 
certain business rules.
Applications can show error messages in many languages according to user 
choices thanks to ASP.NET Core MVC's support for localizing error messages.

STEP-10

Navigated to the Details Method: Find and examine the Details method's implementation in the application.
Usually, this technique takes care of the retrieval and presentation of comprehensive data for a particular item.
investigated how the Delete method was implemented inside the app and looked at it. This technique typically
handles the deletion of a particular entity, guaranteeing accurate data erasure.
Examined the logic of the code: examined the logical reasoning behind the Details and Delete methods' code. 
This entails being aware of how the Delete method handles deletions and how data is retrieved for Details.
Error handling was checked to make sure it was implemented correctly, particularly when managing user requests 
for deletion or more information. When requested entities are not discovered or deletion errors arise, the methods
ought to respond to those situations politely.
Verified Security Measures: These measures verify that appropriate authorization and authentication checks are in
place to prevent unauthorized access to the Details and Delete features, among other security precautions.

Observations: 
It appears that the Details method retrieves information from the database and presents it in a detailed view. 
The effectiveness and accuracy with which data is retrieved for presenting is one example of an observation.
The reasoning behind the Delete method's handling of entity deletions would be scrutinized. This covers any more 
business rules related to deletion, confirmation prompts, and how deletion problems should be handled.
Security Checks: Information about the application's overall security posture can be gained by noting how 
security checks are implemented, such as making sure that only authorized users can access and make deletions.






