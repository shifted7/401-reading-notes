# Reading 28: Claims
## MS Docs: Claims-based Authorization in ASP.NET Core
- When an identity is created, it can be assigned claims, issued by a trusted party.
  - Claim is a name value pair that represents what subject is (not what it can do).
    - Like a driver's license
    - Authorization can check the value of a claim and allow access to a resource based upon that value
  - An identity can contain multiple claims with multiple values and can contain multiple claims of the same type

### Adding claims checks
- Claims-based authorization checks are declarative
  - The developer embeds checks within their code, against a controller or action within a controller
    - Specifies claims which the current user must possess, or the value the claim must hold to access the requested resource.
    - Claims requirements are policy-based
      - The developer must build and register a policy expressing the claims requirements
    - Ex: In ConfigureServices, after AddMvc:
      - services.AddAuthorization(options => { options.AddPolicy("EmployeeOnly", policy => policy.RequireClaim("EmployeeNumber"));});
      - The EmployeeOnly policy checks for the presence of an EmployeeNumber claim on the current identity
    - The policy is then applied using [Authorize(Policy="EmployeeOnly")] tag above the controller class or above an action
    
### Multiple Policy Evaluation
- If multiple policies are applied to a controller or action, all policies must pass before access is granted
