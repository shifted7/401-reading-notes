# Reading 29: Policies
## MS Docs: Policy-based authorization in ASP.NET Core
- Implement in controller, above action:
  - [Authorize(Policy="AgeOver21")]
- Implement in Razor Pages:
  - In cshtml.cs file, above class:
    - [Authorize(Policy="AgeOver21")]
## Custom Authorization Policy Providers using IAuthorizationPolicyProvider in ASP.NET Core
