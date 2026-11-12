<pre style="font-family: monospace; font-size: 10px; line-height: 10; overflow-x: auto; color: #ffffff;">
███████╗██████╗ ██╗ ██████╗██╗  ██╗   ███╗   ███╗ █████╗  ██████╗  █████╗  ██████╗ ███╗   ██╗ █████╗ 
██╔════╝██╔══██╗██║██╔════╝██║ ██╔╝   ████╗ ████║██╔══██╗██╔════╝ ██╔══██╗██╔════╝ ████╗  ██║██╔══██╗
█████╗  ██████╔╝██║██║     █████╔╝    ██╔████╔██║███████║██║  ███╗███████║██║  ███╗██╔██╗ ██║███████║
██╔══╝  ██╔══██╗██║██║     ██╔═██╗    ██║╚██╔╝██║██╔══██║██║   ██║██╔══██║██║   ██║██║╚██╗██║██╔══██║
███████╗██║  ██║██║╚██████╗██║  ██╗   ██║ ╚═╝ ██║██║  ██║╚██████╔╝██║  ██║╚██████╔╝██║ ╚████║██║  ██║
╚══════╝╚═╝  ╚═╝╚═╝ ╚═════╝╚═╝  ╚═╝   ╚═╝     ╚═╝╚═╝  ╚═╝ ╚═════╝ ╚═╝  ╚═╝ ╚═════╝ ╚═╝  ╚═══╝╚═╝  ╚═╝
</pre>

## ABOUT

I'm a Software Engineering student with a particular interest in software architecture and backend development. I enjoy understanding how systems are organized and structured, and building practical solutions that other developers can easily understand, maintain, and evolve. These are concepts I've been exploring through my projects with .NET.

When I'm not studying or coding, I'm probably playing guitar. 🎸

## STACK

![C#](https://img.shields.io/badge/C%23-239120?style=for-the-badge)
![.NET](https://img.shields.io/badge/.NET-512BD4?style=for-the-badge)
![ASP.NET Core](https://img.shields.io/badge/ASP.NET_Core-512BD4?style=for-the-badge)
![EF Core](https://img.shields.io/badge/EF_Core-512BD4?style=for-the-badge)
![SQL Server](https://img.shields.io/badge/SQL_Server-CC2927?style=for-the-badge)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge)

## PROJECTS

### 📦 Storage System

A storage management application built with C# and .NET, focused on software architecture, domain modeling, and maintainable code. Developed as a practical study of how to structure applications, organize responsibilities, and apply software design principles.

**Features**
- Brand and product CRUD
- Stock management
- Relational data persistence
- Rich-domain model

**Architecture & Design**

The solution follows a layered architecture, separating business rules, application logic, and infrastructure concerns.

```text
StorageSystem/
├── StorageSystem.Domain/
│   ├── Entities/
│   ├── Exceptions/
│   └── Guards/
│
├── StorageSystem.Application/
│   ├── Services/
│   └── Repository/
│
├── StorageSystem.Infrastructure/
│   ├── Data/
│   └── Repository/
│
├── StorageSystem.Console/
│   └── UI/
│
└── StorageSystem.Tests/
    ├── Domain/
    ├── Application/
    └── Infrastructure/
```

**Key Design Decisions**

- **Clean Architecture:** strict separation of concerns between Domain, Application, and Infrastructure.
- **Rich Domain Model:** encapsulated entities with guarded state changes, centralizing business rules.
- **Dependency Inversion:** the Domain project has zero external dependencies (not even EF Core), ensuring pure, framework-agnostic business rules.
- **Repository Pattern:** abstracting persistence operations to keep application services decoupled from data access implementations.
- **Automated Testing:** unit tests validating domain invariants and application orchestration.

**Tech Stack**

![C#](https://img.shields.io/badge/C%23-239120?style=flat&logo=csharp&logoColor=white)
![.NET](https://img.shields.io/badge/.NET-512BD4?style=flat&logo=dotnet&logoColor=white)
![EF Core](https://img.shields.io/badge/EF_Core-512BD4?style=flat&logo=dotnet&logoColor=white)
![SQL Server](https://img.shields.io/badge/SQL_Server-CC2927?style=flat&logo=microsoftsqlserver&logoColor=white)
![xUnit](https://img.shields.io/badge/xUnit-512BD4?style=flat)

[View Repository](https://github.com/kkcire/storage-system)

### 📫 Contact
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/erick-magagna/)
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:erickmagagna84@gmail.com)
