## Domain Layer

### Aggregates
This module follows the [Entity Best Practices & Conventions](https://docs.abp.io/en/abp/latest/Best-Practices/Entities) guide.
- `FileDescriptor`
- `DirectoryDescriptor`

### Repositories
This module follows the [Repository Best Practices & Conventions](https://docs.abp.io/en/abp/latest/Best-Practices/Repositories) guide.
Following custom repositories are defined for this module:
- `IFileDescriptorRepository`
- `IDirectoryDescriptorRepository`

### Domain Services
This module follows the [Domain Services Best Practices & Conventions](https://docs.abp.io/en/abp/latest/Best-Practices/Domain-Services) guide.
- `FileManager`
- `DirectoryManager`

### Settings
This module doesn't define any setting.

### Features
- `FileManagement.Enable` : Enable file management system in the application.
- `FileManagement.StorageSize` : Set maximum storage size in bytes. Zero or null will be unlimited.

## Application Layer

### Application Services
- `FileDescriptorAppService` (implements 'IFileDescriptorAppService')
- `DirectoryDescriptorAppService` (implements 'IDirectoryDescriptorAppService')

### Permissions
- `FileManagement.DirectoryDescriptor`: Directory
- `FileManagement.DirectoryDescriptor.Create`: Create
- `FileManagement.DirectoryDescriptor.Update`: Update
- `FileManagement.DirectoryDescriptor.Delete`: Delete
- `FileManagement.FileDescriptor`: File
- `FileManagement.FileDescriptor.Create`: Create
- `FileManagement.FileDescriptor.Update`: Update
- `FileManagement.FileDescriptor.Delete`: Delete

## Database Providers

### Common
#### Connection String
This module uses `FileManagement` for the connection string name. If you don't define a connection string with this name, it fallbacks to the `Default` connection string.

See the [connection strings](https://docs.abp.io/en/abp/latest/Connection-Strings) documentation for details.

#### Entity Framework Core
Tables

- `FmDirectoryDescriptors`
- `FmFileDescriptors`

#### MongoDB
Collections
- `FmFileDescriptors`
- `FmDirectoryDescriptors`

