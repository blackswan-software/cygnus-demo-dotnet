# Cygnus Demo — eShop (.NET/C#)

Demonstrating [Cygnus](https://cygnus.blackswan-software.ai) verified API tokens
improving AI-generated code quality on .NET enterprise applications.

## Why .NET Enterprise?

Banks, insurance companies, property management firms, and government contractors
run massive .NET codebases. These organizations are adopting AI coding tools but
cannot afford hallucinated API calls — wrong parameters in financial transaction
code, incorrect Entity Framework queries, or broken Stripe integration means
regulatory risk and production outages.

Cygnus provides cryptographically verified function signatures so AI models
generate code that matches the **actual compiled API**, not what the model
thinks the API looks like.

## Dependency Coverage

### Have Cygnus tokens (10 libs, 55,000+ tokens)
- `Stripe.net` (16,643 tokens) — payment processing
- `Microsoft.EntityFrameworkCore` (10,483 tokens) — ORM
- `EPPlus` (6,940 tokens) — Excel generation
- `MongoDB.Driver` (4,954 tokens) — document DB
- `Microsoft.Data.SqlClient` (3,190 tokens) — SQL Server
- `MediatR` — CQRS/mediator pattern
- `FluentValidation` — input validation
- `Serilog` — structured logging
- `AutoMapper` — object mapping
- `Newtonsoft.Json` — JSON serialization
- `RabbitMQ.Client` — message queue
- `Dapper` — micro-ORM

### Compiling now (3 libs)
- `Polly` — resilience/retry policies
- `StackExchange.Redis` — caching
- `Swashbuckle.AspNetCore` — OpenAPI/Swagger

**Target: 100% dependency coverage.**

## Enterprise Value Proposition

| Without Cygnus | With Cygnus |
|---------------|-------------|
| AI guesses EF Core query syntax | Verified DbContext, LINQ, migration APIs |
| Wrong Stripe charge parameters | Exact PaymentIntent.Create signature |
| SqlClient connection string errors | Verified SqlConnection constructor |
| Hope-based code review | Cryptographic proof against compiled source |

## Setup

```bash
# Install Cygnus CLI
curl -fsSL https://install.cygnus.blackswan-software.ai | sh

# Bootstrap Cygnus tokens for project deps
python3 cygnus/bootstrap.py
```

## License

Demo scripts: MIT
Cygnus verified tokens: proprietary (BlackSwan Software Corp)
