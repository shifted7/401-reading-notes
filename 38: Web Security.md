# Reading 38: Web Security
## Why do we need HTTPS
- 3 reasons:
  - Privacy, integrity, and identification
- Privacy
  - Encrypts your message so that evil crabs cannot read it
- Integrity
  - Encryption lets you know if the message was intercepted and changed
- Identification
  - SSL certificate tells you that you have connected to the correct location

## .NET OWASP Cheat Sheet
- .NET is kept up-to-date by Microsoft via Windows Update
- Individual frameworks are kept up-to-date using NuGet
- Check for security announcements at https://github.com/dotnet/announcements/issues?q=is%3Aopen+is%3Aissue+label%3ASecurity

### Data Access
- Use parameterized SQL commands for all data access, without exception
- Do not use SqlCommand with a string parameter made up of a concatenated SQL string
- Whitelist values coming from users via enums, tryparse, or lookup values
- Apply principles of least privilege when setting up the Database User
- Use Entity Framework
- When using SQL server, use integrated authentication vs SQL authentication
- Use Always Encrypted where possible for sensitive data

### Encryption
- Never, ever write your own encryption
- Strongest general hashing algorithm is System.Security.Cryptography.SHA512
- Strongest password hashing algorithm in .NET framework is System.Security.Cryptography.Rfc2898DeriveBytes
- Strongest password hashing algorithm in .NET Core is Microsoft.AspNetCore.Cryptography.KeyDerivation.Pbkdf2
- Salt your passwords
- Make sure your app can support future changes of crypto algorithms
- Use Nuget to keep packages up to date







