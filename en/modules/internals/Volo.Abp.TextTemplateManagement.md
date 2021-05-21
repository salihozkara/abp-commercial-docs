## Domain Layer

### Aggregates
This module follows the [Entity Best Practices & Conventions](https://docs.abp.io/en/abp/latest/Best-Practices/Entities) guide.
- `TextTemplateContent`

### Repositories
This module follows the [Repository Best Practices & Conventions](https://docs.abp.io/en/abp/latest/Best-Practices/Repositories) guide.
Following custom repositories are defined for this module:
- `ITextTemplateContentRepository`


### Settings
This module doesn't define any setting.

### Features
- `TextManagement.Enable` : Enable text management system in the application.

## Application Layer

### Application Services
- `TemplateContentAppService` (implements 'ITemplateContentAppService')
- `TemplateDefinitionAppService` (implements 'ITemplateDefinitionAppService')

### Permissions
- `TextTemplateManagement.TextTemplates`: Text Templates
- `TextTemplateManagement.TextTemplates.EditContents`: Edit Contents

## Database Providers

### Common
#### Connection String
This module uses `TextTemplateManagement` for the connection string name. If you don't define a connection string with this name, it fallbacks to the `Default` connection string.

See the [connection strings](https://docs.abp.io/en/abp/latest/Connection-Strings) documentation for details.

#### Entity Framework Core
Tables

- `AbpTextTemplateContents`

#### MongoDB
Collections

- `AbpTextTemplates`

