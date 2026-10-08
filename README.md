<h1 align="center">Hi, I'm Liam Swile 👋</h1>

<p align="center">
  <b>.NET developer in training</b> building cloud-hosted, tested, containerised web applications.<br/>
  C# · ASP.NET Core · Azure · SQL Server · Docker
</p>

<p align="center">
  <!-- TODO: replace YOUR-LINKEDIN and add your email/portfolio if you want them public -->
  <a href="https://www.linkedin.com/in/liam-swile-a4a951331"><img src="https://img.shields.io/badge/LinkedIn-Connect-0A66C2?logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
  <a href="mailto:dswile9@gmail.com"><img src="https://img.shields.io/badge/Email-Contact%20me-D14836?logo=gmail&logoColor=white" alt="Email"/></a>
</p>

---

## 🔭 About me

I'm a software development student who enjoys the full path from idea to running product: designing the data model, building the API and UI, writing tests, and getting it deployed. My recent work covers three different .NET architectures: a **cloud-native Azure app**, a **secure role-based MVC system**, and a **containerised API + Blazor platform with CI**.

- 🌱 Currently deepening my knowledge of cloud architecture, design patterns and automated testing
- 💼 Looking for **junior / graduate .NET developer** opportunities
- 💬 Ask me about: ASP.NET Core, Entity Framework Core, Azure Storage and Functions, JWT auth, Docker

## 🛠️ Tech stack

**Languages & frameworks**

![C#](https://img.shields.io/badge/C%23-239120?logo=csharp&logoColor=white)
![.NET](https://img.shields.io/badge/.NET%208%20%2F%2010-512BD4?logo=dotnet&logoColor=white)
![ASP.NET Core](https://img.shields.io/badge/ASP.NET%20Core-512BD4?logo=dotnet&logoColor=white)
![Blazor](https://img.shields.io/badge/Blazor-512BD4?logo=blazor&logoColor=white)
![Razor MVC](https://img.shields.io/badge/MVC%20%2F%20Razor-512BD4?logo=dotnet&logoColor=white)
![Bootstrap](https://img.shields.io/badge/Bootstrap-7952B3?logo=bootstrap&logoColor=white)

**Cloud, data & DevOps**

![Azure](https://img.shields.io/badge/Azure-0078D4?logo=microsoftazure&logoColor=white)
![Azure Functions](https://img.shields.io/badge/Azure%20Functions-0062AD?logo=azurefunctions&logoColor=white)
![SQL Server](https://img.shields.io/badge/SQL%20Server-CC2927?logo=microsoftsqlserver&logoColor=white)
![EF Core](https://img.shields.io/badge/Entity%20Framework%20Core-512BD4?logo=dotnet&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?logo=githubactions&logoColor=white)
![Swagger](https://img.shields.io/badge/Swagger%20%2F%20OpenAPI-85EA2D?logo=swagger&logoColor=black)

**Testing & tools**

![xUnit](https://img.shields.io/badge/xUnit-512BD4?logo=dotnet&logoColor=white)
![Moq](https://img.shields.io/badge/Moq-5C2D91)
![Git](https://img.shields.io/badge/Git-F05032?logo=git&logoColor=white)
![Visual Studio](https://img.shields.io/badge/Visual%20Studio-5C2D91?logo=visualstudio&logoColor=white)

---

## 🚀 Featured projects

### 1. Logistics Management Platform — API + Blazor + Docker + CI
`.NET 10` · `ASP.NET Core Web API` · `Blazor Server` · `EF Core` · `SQL Server` · `Docker Compose` · `GitHub Actions`

A logistics contract and service-request management platform made of a REST API, a Blazor Server frontend and an integration-test project, all brought up with a single `docker compose up`.

- 🔐 **JWT authentication**: every endpoint except login requires a signed bearer token; the Blazor app injects it into outgoing calls through a delegating handler
- 🧩 **Three Gang-of-Four patterns** in real use: **Factory Method** (freight vs driver contracts), **Observer** (compliance logging and notifications on contract status changes) and **Decorator** (SLA validation and USD→ZAR conversion layered onto service requests)
- 🗄️ **Repository pattern** over five repositories, plus a `ContractWorkflowService` that enforces valid status transitions (`Draft → Active → Completed`)
- 💱 Live currency conversion through ExchangeRate-API, and PDF contract upload
- ✅ **18 xUnit integration tests** run against the real HTTP pipeline with an in-memory database, executed on every push by a **GitHub Actions** workflow
- 📄 Swagger/OpenAPI documentation

> 🔗 Repository: [LMSA---Logistics-Management-System-Application](https://github.com/ST10438679/LMSA---Logistics-Management-System-Application)

---

### 2. Cloud Retail Application — Azure Storage + Functions
`.NET 8` · `ASP.NET Core MVC` · `Azure Table / Blob / Queue / File Share` · `Azure Functions` · `Azure SQL` · `Azure App Service`

An e-commerce style web app (customers, products, orders, cart and contracts) that uses the full range of **Azure Storage** services, with a separate **Azure Functions** app handling uploads and background work.

- ☁️ Four dedicated storage services (Table, Blob, Queue, File Share) registered with dependency injection
- ⚡ **Azure Functions** (isolated worker, Application Insights enabled) for customer inserts to Table Storage, image and video uploads to Blob Storage, file-share uploads and queue messaging
- 👥 Role-based experience for **admin** and **customer** users, with session-based login
- 🗄️ Relational data in **Azure SQL** through EF Core; deployed to **Azure App Service**
- 🎥 Walkthrough videos of the app and the Azure services were recorded for assessment

> 🔗 Repository: [CRA---Cloud-Retail-Application](https://github.com/ST10438679/CRA---Cloud-Retail-Application)

---

### 3. Contract Monthly Claim System (CMCS) — Secure role-based MVC
`.NET 8` · `ASP.NET Core MVC` · `EF Core` · `SQL Server` · `QuestPDF` · `xUnit` · `Moq`

A claims workflow for lecturers' monthly work: lecturers submit claims with supporting documents, which then move through **Programme Coordinator** and **Academic Manager** approval, with **HR** handling invoicing and reporting.

- 👤 Four-role access model (Lecturer, Programme Coordinator, Academic Manager, HR) with controllers and views per role
- 🔒 **Supporting documents are encrypted at rest** by an `EncryptionService` and stored outside the web root to block unauthorised access
- 🧾 **Automated PDF invoice generation** with QuestPDF
- 🎨 Colour-coded claim statuses for quick reading, and a two-stage approval flow
- ✅ Unit tests with xUnit and Moq covering the controller logic and claim model
- 🔁 Iterated across three submission parts, incorporating lecturer feedback (documented in the project README)

> 🔗 Repository: [CMCS---Contract-Monthly-Claim-System](https://github.com/ST10438679/CMCS---Contract-Monthly-Claim-System)

---

## 🧠 What these projects show

| Skill | Where I've applied it |
|---|---|
| REST API design and JWT security | Logistics Management Platform |
| Design patterns (Factory, Observer, Decorator, Repository) | Logistics Management Platform |
| Cloud architecture (Azure Storage, Functions, App Service) | Cloud Retail Application |
| Automated testing and CI | Logistics platform (integration + GitHub Actions), CMCS (unit + mocks) |
| Containerisation | Docker Compose with SQL Server 2022, API and Blazor frontend |
| Application security (encryption, role-based access) | CMCS, Logistics platform |
| Working from feedback and documenting changes | CMCS, across three submission parts |

---

<p align="center">
  <i>Thanks for stopping by. If you're hiring for a junior .NET role, I'd love to chat.</i>
</p>
