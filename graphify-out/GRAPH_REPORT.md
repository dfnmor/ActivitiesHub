# Graph Report - EventsHub  (2026-10-03)

## Corpus Check
- cluster-only mode — file stats not available

## Summary
- 407 nodes · 613 edges · 23 communities (19 shown, 4 thin omitted)
- Extraction: 99% EXTRACTED · 1% INFERRED · 0% AMBIGUOUS · INFERRED: 7 edges (avg confidence: 0.85)
- Token cost: 0 input · 0 output

## Graph Freshness
- Built from commit: `dbb95243`
- Run `git rev-parse HEAD` and compare to check if the graph is stale.
- Run `graphify update .` after code changes (no API cost).

## Community Hubs (Navigation)
- EventsRpcClient
- EventsHub/package.json
- EventsHub.Persistence
- .GetEventsAsync
- EventsHub.Api
- 20260831233114_InitialCreate.Designer.cs
- compilerOptions
- EventsHubBaseContoller
- Event
- devDependencies
- compilerOptions
- AppDbContext
- Handler
- Event
- Command
- IRequest
- https
- EventsHub.OpenApi
- WeatherForecast
- dependencies
- Handler
- tsconfig.json
- index.d.ts

## God Nodes (most connected - your core abstractions)
1. `Event` - 25 edges
2. `EventsRpcClient` - 20 edges
3. `WeatherForecastRpcClient` - 19 edges
4. `compilerOptions` - 18 edges
5. `ApiException` - 15 edges
6. `compilerOptions` - 15 edges
7. `AppDbContext` - 14 edges
8. `Event` - 13 edges
9. `EventsHub.Persistence` - 11 edges
10. `EventsHub.Api` - 10 edges

## Surprising Connections (you probably didn't know these)
- `GlobalTestSetup` --references--> `AppDbContext`  [EXTRACTED]
  tests/EventsHub.UnitTests/GlobalTestSetup.cs → src/EventsHub.Persistence/AppDbContext.cs
- `EventsHub.UnitTests` --references--> `net10.0`  [EXTRACTED]
  tests/EventsHub.UnitTests/EventsHub.UnitTests.csproj → src/EventsHub.Api/EventsHub.Api.csproj
- `EventsHub.UnitTests` --references--> `Microsoft.NET.Sdk`  [EXTRACTED]
  tests/EventsHub.UnitTests/EventsHub.UnitTests.csproj → src/EventsHub.Domain/EventsHub.Domain.csproj
- `Handler` --references--> `AppDbContext`  [EXTRACTED]
  src/EventsHub.Application/Events/Command/CreateEvent.cs → src/EventsHub.Persistence/AppDbContext.cs
- `Handler` --references--> `AppDbContext`  [EXTRACTED]
  src/EventsHub.Application/Events/Command/DeleteEvent.cs → src/EventsHub.Persistence/AppDbContext.cs

## Import Cycles
- None detected.

## Communities (23 total, 4 thin omitted)

### Community 0 - "EventsRpcClient"
Cohesion: 0.07
Nodes (20): EventsHub.OpenApi.Client, ApiException, Headers, Response, Result, StatusCode, DateFormatConverter, EventsRpcClient (+12 more)

### Community 1 - "EventsHub/package.json"
Cohesion: 0.06
Nodes (39): axios, @babel/core, babel-plugin-react-compiler, @emotion/react, @emotion/styled, eslint, @eslint/js, eslint-plugin-react-hooks (+31 more)

### Community 2 - "EventsHub.Persistence"
Cohesion: 0.13
Nodes (8): EventsHub.Domain, EventsHub.Application.Events.Command, EventsHub.Application.Events.Queries, EventsHub.Application.Events.Commands, EventsHub.UnitTests, EventsHub.Persistence, EventsHub.Application.Core, MappingProfiles

### Community 4 - "EventsHub.Api"
Cohesion: 0.14
Nodes (24): AutoMapper (13.0.1), coverlet.collector (6.0.4), MediatR (14.2.0), Microsoft.AspNetCore.Mvc.NewtonsoftJson (10.0.11), Microsoft.AspNetCore.OpenApi (10.0.11), Microsoft.EntityFrameworkCore.Design (10.0.11), Microsoft.NET.Test.Sdk (17.14.0), Moq (4.20.72) (+16 more)

### Community 5 - "20260831233114_InitialCreate.Designer.cs"
Cohesion: 0.12
Nodes (3): EventsHub.Persistence.Migrations, InitialCreate, AppDbContextModelSnapshot

### Community 6 - "compilerOptions"
Cohesion: 0.10
Nodes (19): compilerOptions, allowArbitraryExtensions, allowImportingTsExtensions, erasableSyntaxOnly, jsx, lib, module, moduleDetection (+11 more)

### Community 7 - "EventsHubBaseContoller"
Cohesion: 0.12
Nodes (5): EventsHub.Api.Controllers, EventsHub.UnitTests.Controllers, EventsHubBaseContoller, Mediator, WeatherForecastController

### Community 8 - "Event"
Cohesion: 0.12
Nodes (16): Event, Category, City, Date, Description, Id, IsCancelled, Latitude (+8 more)

### Community 9 - "devDependencies"
Cohesion: 0.12
Nodes (17): devDependencies, @babel/core, babel-plugin-react-compiler, eslint, @eslint/js, eslint-plugin-react-hooks, eslint-plugin-react-refresh, globals (+9 more)

### Community 10 - "compilerOptions"
Cohesion: 0.12
Nodes (16): compilerOptions, allowImportingTsExtensions, erasableSyntaxOnly, lib, module, moduleDetection, noEmit, noFallthroughCasesInSwitch (+8 more)

### Community 11 - "AppDbContext"
Cohesion: 0.16
Nodes (5): AppDbContext, Events, DbInitializer, GlobalTestSetup, AppDbContext

### Community 12 - "Handler"
Cohesion: 0.21
Nodes (4): Handler, GetEventList, Handler, Query

### Community 13 - "Event"
Cohesion: 0.15
Nodes (11): Event, Category, City, Date, Description, Id, IsCancelled, Latitude (+3 more)

### Community 15 - "IRequest"
Cohesion: 0.20
Nodes (9): Command, Event, CreateEvent, Command, Event, EditEvent, GetEventdetails, Query (+1 more)

### Community 16 - "https"
Cohesion: 0.20
Nodes (9): ASPNETCORE_ENVIRONMENT, applicationUrl, commandName, dotnetRunMessages, environmentVariables, launchBrowser, profiles, https (+1 more)

### Community 17 - "EventsHub.OpenApi"
Cohesion: 0.22
Nodes (8): ASPNETCORE_ENVIRONMENT, applicationUrl, commandName, environmentVariables, launchBrowser, profiles, EventsHub.OpenApi, $schema

### Community 18 - "WeatherForecast"
Cohesion: 0.25
Nodes (6): EventsHub.Api, WeatherForecast, Date, Summary, TemperatureC, TemperatureF

### Community 19 - "dependencies"
Cohesion: 0.25
Nodes (8): dependencies, @emotion/react, @emotion/styled, @fontsource/roboto, @mui/icons-material, @mui/material, react, react-dom

### Community 20 - "Handler"
Cohesion: 0.29
Nodes (4): Command, Id, DeleteEvent, Handler

## Knowledge Gaps
- **155 isolated node(s):** `Activity`, `EventsHub.OpenApi.Client`, `Headers`, `Response`, `Result` (+150 more)
  These have ≤1 connection - possible missing edges. (Counts symbols only; 210 node(s) total have ≤1 connection when file, concept and rationale nodes are included.)
- **4 thin communities (<3 nodes) omitted from report** — run `graphify query` to explore isolated nodes.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **Why does `Event` connect `Event` to `AppDbContext`, `.GetEventsAsync`, `Handler`, `IRequest`?**
  _High betweenness centrality (0.058) - this node is a cross-community bridge._
- **Why does `AppDbContext` connect `AppDbContext` to `EventsHub.Persistence`, `Handler`, `Event`, `Command`, `Handler`?**
  _High betweenness centrality (0.050) - this node is a cross-community bridge._
- **Why does `EventsHub.Persistence` connect `EventsHub.Persistence` to `20260831233114_InitialCreate.Designer.cs`?**
  _High betweenness centrality (0.025) - this node is a cross-community bridge._
- **What connects `Activity`, `EventsHub.OpenApi.Client`, `Headers` to the rest of the system?**
  _155 weakly-connected nodes found - possible documentation gaps or missing edges._
- **Should `EventsRpcClient` be split into smaller, more focused modules?**
  _Cohesion score 0.07373271889400922 - nodes in this community are weakly interconnected._
- **Should `EventsHub/package.json` be split into smaller, more focused modules?**
  _Cohesion score 0.05603864734299517 - nodes in this community are weakly interconnected._
- **Should `EventsHub.Persistence` be split into smaller, more focused modules?**
  _Cohesion score 0.13105413105413105 - nodes in this community are weakly interconnected._