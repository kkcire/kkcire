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

### 1. STORAGE SYSTEM

A console-based storage management application built with C# and .NET, focused on software architecture, domain modeling, and maintainable code. Built as a practical study of how to structure applications and organize responsibilities.

**Features**
- Brand and product management: register, update (full or partial), delete, search, and list
- Products linked to brands; a brand can't be deleted while it has products
- Interactive terminal interface built with Spectre.Console

**Key Design Decisions**
- **Clean Architecture:** separates business rules, application logic, and infrastructure concerns into distinct layers, with dependencies pointing inward toward the Domain.
- **Rich Domain Model:** private setters and static factories; entities enforce their own invariants through guard clauses.
- **Repository Pattern & Dependency Inversion:** repository interfaces live in Application and are implemented in Infrastructure, so services never depend on EF Core.
- **Database integrity:** unique indexes, restricted deletes, and EF Core migrations applied at startup.
- **Testing:** unit tests for the domain, plus integration tests against a real SQL Server. Each test gets its own temporary database built from the real migrations, covering services, repositories, and constraints.

---

<details>
<summary><b>Project Architecture Tree</b></summary>

```text
StorageSystem/
├── src/
│   ├── StorageSystem.Application/
│   │   ├── Repository/
│   │   └── Services/
│   │
│   ├── StorageSystem.Domain/
│   │   ├── Entities/
│   │   ├── Exceptions/
│   │   └── Guards/
│   │
│   ├── StorageSystem.Infrastructure/
│   │   ├── Data/
│   │   ├── Repository/
│   │   └── Migrations/
│   │
│   └── StorageSystem.Console/
│       └── UI/
│
└── test/
    └── StorageSystem.Tests/
        ├── Domain/
        ├── Application/
        └── Infrastructure/
```
</details>

---

### **Tech Stack**

![C#](https://img.shields.io/badge/C%23-239120?style=flat)
![.NET](https://img.shields.io/badge/.NET_10-512BD4?style=flat)
![EF Core](https://img.shields.io/badge/EF_Core-512BD4?style=flat)
![SQL Server](https://img.shields.io/badge/SQL_Server-CC2927?style=flat)
![xUnit](https://img.shields.io/badge/xUnit-512BD4?style=flat)
![Spectre.Console](https://img.shields.io/badge/Spectre.Console-5E5E5E?style=flat)

**[Explore Project](https://github.com/kkcire/storage-system)**

## CONTACT
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/erick-magagna/)
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:erickmagagna84@gmail.com)
