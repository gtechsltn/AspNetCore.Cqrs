# ASP.NET Core CQRS
+ https://levelup.gitconnected.com/cqrs-in-asp-net-with-separate-read-write-models-using-mediatr-b2fa32be9e65
+ https://betterprogramming.pub/choosing-a-cqrs-architecture-that-works-for-you-02619555b0a0
+ https://betterprogramming.pub/domain-driven-design-domain-events-and-integration-events-in-net-5a2a58884aaa
+ https://betterprogramming.pub/domain-driven-design-a-walkthrough-of-building-an-aggregate-c84113aa9975

## Clean Architecture
+ https://github.com/gtechsltn/AspNetCore.CleanArchitecture
  + Clean Architecture
  + Domain-Driven Design
  + High test coverage
  + SOLID principles
  + Containerisation
  + Code-First database management
  + Enforced code styles
  + API tests
  + Architecture tests
  + Automated acceptance testing

## ASP.NET Core CQRS
+ https://github.com/gtechsltn/AspNetCore.Cqrs

## Sample eCommerce application using Domain-Driven Design
+ https://github.com/gtechsltn/DDDMart

## .NET Audit Implementation via the Entity Framework Change Tracker
+ https://github.com/gtechsltn/EntityFramework.Audit
+ https://levelup.gitconnected.com/net-audit-implementation-via-the-entity-framework-change-tracker-3436854fd613

# ASP.NET Core CQRS

**ASP.NET Core** API setup using Command Query Responsibility Segregation (CQRS). 
The solution follows the 'Different Read/Write Models, Single Database' approach described here: https://medium.com/better-programming/choosing-a-cqrs-architecture-that-works-for-you-02619555b0a0

**MediatR** is used to implement Command, Query and Domain Event handling in the project.

- **Write Side**: Entity Framework Core is used for Commands
- **Read Side**: Dapper is used for Queries

The setup follows important modern development principles described here: https://github.com/matt-bentley/CleanArchitecture

The application extends the typical *Weather Forecast* example provided in default .NET project templates and contains the following components:

- **API** - ASP.NET 7 REST API with Swagger support
- **Database** - SQL Server database integration via Entity Framework Core and Dapper
- **Migrations** - Code-First database migrations managed using a console application
  

## Quick Start

1. Start local database in Docker

```bash
docker-compose --profile dev up -d
```

2. Run the **AspNetCore.Cqrs.Migrations** project to deploy database schema
3. Run the **AspNetCore.Cqrs.Api** projects to debug the API and view Swagger

