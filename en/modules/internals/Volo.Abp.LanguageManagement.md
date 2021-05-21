## Domain Layer

### Aggregates
This module follows the [Entity Best Practices & Conventions](https://docs.abp.io/en/abp/latest/Best-Practices/Entities) guide.
- `Language`
- `LanguageText`

### Repositories
This module follows the [Repository Best Practices & Conventions](https://docs.abp.io/en/abp/latest/Best-Practices/Repositories) guide.
Following custom repositories are defined for this module:
- `ILanguageRepository`
- `ILanguageTextRepository`


### Settings
This module doesn't define any setting.

### Features
- `LanguageManagement.Enable` : Enable language management system in the application.


## Database Providers

### Common
#### Connection String
This module uses `AbpLanguageManagement` for the connection string name. If you don't define a connection string with this name, it fallbacks to the `Default` connection string.

See the [connection strings](https://docs.abp.io/en/abp/latest/Connection-Strings) documentation for details.

#### Entity Framework Core
Tables

- `AbpLanguages`
- `AbpLanguageTexts`

#### MongoDB
Collections

- `AbpLanguageTexts`
- `AbpLanguages`

