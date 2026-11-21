<pre>
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

## FEATURED PROJECT

### ⚙️ STORAGE SYSTEM

A console-based storage management application built with C# and .NET, focused on software architecture, domain modeling, and maintainable code. Built as a practical study of how to structure applications and organize responsibilities.

**Features**
- Brand and product management: register, update (full or partial), delete, search, and list
- Interactive terminal interface built with Spectre.Console

**Key Design Decisions**
**Architectural choices**
- **Clean Architecture:** Kept the domain completely isolated from infrastructure and UI using SOLID principles. Uses Repository Pattern so the Application layer only talks to interfaces, never touching EF Core directly.
- **Rich Domain Model:** No anemic classes with open setters. Entities protect their own state using private setters, static factories, and guard clauses so invalid states can't exist.
- **SQL Server Integration Tests:** Unit tests cover the domain, while integration tests spin up temporary databases from real migrations to validate T-SQL constraints and engine-specific behavior — avoiding in-memory providers that hide database quirks.

<details>
<summary><h4><b>Project Architecture Tree<h4></b></summary>

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

**Tech Stack**

![C#](https://img.shields.io/badge/C%23-239120?style=flat)
![.NET](https://img.shields.io/badge/.NET_10-512BD4?style=flat)
![EF Core](https://img.shields.io/badge/EF_Core-512BD4?style=flat)
![SQL Server](https://img.shields.io/badge/SQL_Server-CC2927?style=flat)
![xUnit](https://img.shields.io/badge/xUnit-512BD4?style=flat)
![Spectre.Console](https://img.shields.io/badge/Spectre.Console-5E5E5E?style=flat)

**[View Project](https://github.com/kkcire/storage-system)**

## OTHER PROJECTS

- **[Hearth](https://github.com/kkcire/hearth)** — Personal finance tracker built to handle credit card billing cycles, installments, and cash-flow vs. accrual accounting rules.
- **[CDB Calculator](https://github.com/kkcire/cdb-calculator)** — Layered console simulator for Brazilian fixed-income returns, featuring a dynamic interest-rate fluctuation model.
- **[C# Survival Guide](https://github.com/kkcire/csharp-survival-guide)** — Structured study repository documenting C# and .NET fundamentals, type system mechanics, and control flow exercises.

## CONTACT
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/erick-magagna/)
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:erickmagagna84@gmail.com)
