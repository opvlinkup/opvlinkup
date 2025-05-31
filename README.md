## 📌.NET EF Core Command Reference Table

| Command | Description | Example |
|--------|-------------|---------|
| `dotnet ef migrations add <Name>` | Adds a new migration with the specified name. | `dotnet ef migrations add InitialCreate` |
| `dotnet ef database update` | Applies the latest migration to the database. | `dotnet ef database update` |
| `dotnet ef database update <Migration>` | Updates the database to a specific migration. | `dotnet ef database update InitialCreate` |
| `dotnet ef migrations remove` | Removes the last added migration (if not applied). | `dotnet ef migrations remove` |
| `dotnet ef database drop` | Drops the database. Confirmation required. | `dotnet ef database drop` |
| `dotnet ef migrations list` | Lists all applied and pending migrations. | `dotnet ef migrations list` |
| `dotnet ef dbcontext list` | Lists all available DbContext classes. | `dotnet ef dbcontext list` |
| `dotnet ef dbcontext info` | Shows information about the active DbContext. | `dotnet ef dbcontext info` |
| `dotnet ef dbcontext scaffold` | Reverse-engineers a database into a model. | `dotnet ef dbcontext scaffold "<ConnectionString>" Microsoft.EntityFrameworkCore.SqlServer -o Models` |
| `dotnet ef dbcontext optimize` | (EF Core 8+) Improves startup performance via source generation. | `dotnet ef dbcontext optimize` |
| `dotnet ef dbcontext script` | Generates SQL script for migrations. | `dotnet ef migrations script` |
| `dotnet ef migrations script <From> <To>` | Generates SQL script between two migrations. | `dotnet ef migrations script InitialCreate AddIndexes` |

| Command Category | .NET CLI Command (Recommended)         | Package Manager Console (PMC) Command | Description                                                                                                                                                                                                                                                                                                                                                                                                                             | Common Opti
