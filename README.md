# Azure Functions Studio

This repository contains the target configuration and SRE runtime files compiled by the **Azure Functions Studio** dashboard module.

## 🚀 Description
Scaffold event-driven Azure Function apps. Generate serverless trigger bindings (Http, Queue, Timer), host settings configurations, and deployment packages.

## 🛠️ Specification Matrix
- **Primary Configuration File**: `/deploy/functions/function.json`
- **Execution Command**: `func azure functionapp publish app`
- **Validation Command**: `func azure functionapp list`

## 📋 How to Run & Validate

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Pradeeptalari14/tp-azure-functions.git
   cd tp-azure-functions
   ```

2. **Run Execution Target:**
   ```bash
   func azure functionapp publish app
   ```

3. **Verify Runtime Stability:**
   ```bash
   func azure functionapp list
   ```

## 🔐 Security & Best Practices
* **Secret Isolation**: Use organization-level secrets (or SSM parameter hooks) rather than hardcoded environment variables inside files.
* **Pull Request Lifecycles**: Protect default branch merges with validation checks before merging code changes.
