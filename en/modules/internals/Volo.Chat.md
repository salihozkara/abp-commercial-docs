## Domain Layer

### Aggregates
This module follows the [Entity Best Practices & Conventions](https://docs.abp.io/en/abp/latest/Best-Practices/Entities) guide.
- `ChatUser`
- `Message`
- `UserMessage`
- `Conversation`

### Repositories
This module follows the [Repository Best Practices & Conventions](https://docs.abp.io/en/abp/latest/Best-Practices/Repositories) guide.
Following custom repositories are defined for this module:
- `IChatUserRepository`
- `IMessageRepository`
- `IUserMessageRepository`
- `IConversationRepository`

### Domain Services
This module follows the [Domain Services Best Practices & Conventions](https://docs.abp.io/en/abp/latest/Best-Practices/Domain-Services) guide.
- `MessagingManager`

### Settings
This module doesn't define any setting.

### Features
This module doesn't define any feature.


## Database Providers

### Common
#### Connection String
This module uses `Chat` for the connection string name. If you don't define a connection string with this name, it fallbacks to the `Default` connection string.

See the [connection strings](https://docs.abp.io/en/abp/latest/Connection-Strings) documentation for details.

#### Entity Framework Core
Tables

- `ChatConversations`
- `ChatMessages`
- `ChatUserMessages`
- `ChatUsers`

#### MongoDB
Collections

- `ChatMessages`
- `ChatUsers`
- `ChatUserMessages`
- `ChatConversations`

