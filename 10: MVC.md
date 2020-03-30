# Reading 10: MVC

## Microsoft Docs: Overview of ASP.NET Core MVC

### What is the MVC pattern?
- Model-View-Controller
- Three main groups of components, helping to achieve separation of concerns.
  - Helps with scalability because it is easier to code, debug, and test something that has a single job.
  - More difficult to maintain code that has dependencies in these different areas.
- User requests are routed to a Controller which is responsible for working with the Model to perform user actions/get query results.
  - The controller chooses the View to display to the user, providing it with Model data as necessary.
  ![](https://docs.microsoft.com/en-us/aspnet/core/mvc/overview/_static/mvc.png?view=aspnetcore-2.2)

#### Model Responsibilities
- Represent the state of the application and any business logic or operations that should be performed by it.
- Strongly-typed views typically use ViewModel types designed to contain the data to display on that view.
  - The controller creates and populates these ViewModel instances from the model.
  
#### View Responsibilities
- 

#### Controller Responsibilities
- Handle user interaction, work with the model, and select a view to render.
  
