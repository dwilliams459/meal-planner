# Architecture (Initial)

## Overview
Meal-prep will likely use a 3-tier approach:
- React UI
- .NET API
- SQL Server

## Modules (planned)
- Meal planning
- Recipe management
- Grocery list / shopping
- Meal prep schedule

## Cross-cutting concerns
- Authentication & authorization
- Validation and error handling
- Logging/telemetry
- Configuration and secrets

## Data
- SQL Server as system of record
- Migrations strategy: TBD (EF Core migrations vs SQL projects/scripts)

## Deployment
TBD (Azure App Service, Container Apps, AKS, etc.)
