# Reading 33: OAuth
## MSFT Docs: Facebook, Google, and external provider authentication in ASP.NET Core
- Each provider has different installation processes
- For Microsoft: services.AddAuthentication().AddMicrosoftAccount(microsoftOptions =>{ microsoftOptions.ClientId = Configuration[], microsoftOptions.ClientSecret = Configuration[]});

## Authenticate with OAuth 2.0 in ASP.NET Core 2.0
- Ex: Github
  - Parts of OAuth we need to configure:
    - Client Id
    - Client secret
    - Redirect URI
    - Authorization Endpoint
    - Token Endpoint
