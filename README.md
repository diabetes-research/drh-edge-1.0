# DRH Edge TS 1.0

## Diabetes Research Hub - Edge Platform (TypeScript Implementation)

[![TypeScript](https://img.shields.io/badge/TypeScript-94.3%25-blue)](https://www.typescriptlang.org/)
[![PLpgSQL](https://img.shields.io/badge/PLpgSQL-3.6%25-336791)](https://www.postgresql.org/)
[![JavaScript](https://img.shields.io/badge/JavaScript-2.1%25-yellow)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![License](https://img.shields.io/badge/license-Open%20Source-green)](LICENSE)

## 📋 Table of Contents

- [DRH Edge TS 1.0](#drh-edge-ts-10)
  - [Diabetes Research Hub - Edge Platform (TypeScript Implementation)](#diabetes-research-hub---edge-platform-typescript-implementation)
  - [📋 Table of Contents](#-table-of-contents)
  - [🔬 Overview](#-overview)
    - [What is DRH Edge?](#what-is-drh-edge)
    - [Use Cases](#use-cases)
  - [✨ Key Features](#-key-features)
    - [🔒 Security \& Privacy](#-security--privacy)
    - [📊 Data Processing](#-data-processing)
    - [🛠️ Developer Experience](#️-developer-experience)
    - [📈 Validation \& Verification](#-validation--verification)
  - [🏗️ Architecture](#️-architecture)
    - [Core Components](#core-components)
  - [📋 Prerequisites](#-prerequisites)
    - [Required Software](#required-software)
    - [System Requirements](#system-requirements)
  - [🚀 Installation](#-installation)
    - [Step 1: Install Deno](#step-1-install-deno)
    - [Step 2: Install surveilr](#step-2-install-surveilr)

## 🔬 Overview

**DRH Edge TS 1.0** is a pure TypeScript implementation of the Diabetes Research Hub Edge platform, built on [surveilr](https://surveilr.com) for secure, local-first clinical data transformation and validation. It enables healthcare researchers to process Continuous Glucose Monitor (CGM) data and clinical files at the edge without cloud dependencies.

### What is DRH Edge?

DRH Edge is designed for researchers who need to:

- **Process sensitive health data locally** with complete privacy and security
- **Transform heterogeneous clinical data** into standardized formats
- **Validate and verify** data quality before analysis or sharing
- **De-identify and anonymize** PHI/PII in compliance with regulations
- **Work offline** without cloud infrastructure dependencies

### Use Cases

- **Clinical Research**: Process CGM data from diabetes studies at the source
- **Data Preparation**: Clean and standardize multi-institutional datasets
- **Privacy-First Analysis**: Analyze sensitive data without cloud transmission
- **Regulatory Compliance**: De-identify data before external sharing
- **Edge Computing**: Run complete ETL pipelines on local workstations

## ✨ Key Features

### 🔒 Security & Privacy

- **Local-first architecture** - All processing happens on your machine
- **PHI/PII de-identification** - HIPAA-compliant data anonymization
- **No cloud dependencies** - Complete offline operation capability
- **Encrypted data handling** - HTTPS for any required external communication

### 📊 Data Processing

- **CGM data transformation** - Support for multiple CGM device formats
- **Automated ETL pipelines** - Extract, Transform, Load workflows
- **Schema validation** - Ensure data quality and consistency
- **Structural normalization** - Handle heterogeneous data structures

### 🛠️ Developer Experience

- **Pure TypeScript** - Type-safe, modern codebase
- **Built on surveilr** - Rust-based, memory-safe foundation
- **Deno runtime** - Secure JavaScript/TypeScript execution
- **SQL-based transformations** - Powerful data manipulation with PLpgSQL

### 📈 Validation & Verification

- **Interactive UI** - Browser-based verification dashboard
- **Data quality reports** - Automated consistency checking
- **Provenance tracking** - Maintain complete data lineage
- **Error detection** - Identify and fix data inconsistencies

## 🏗️ Architecture

![drh-edge-architecture](/diabetes-research-hub/assets/drh-edge-architecture.png)

### Core Components

1. **Surveilr Engine**: Rust-based data ingestion and processing
2. **TypeScript Modules**: Business logic and data transformation
3. **PLpgSQL Scripts**: Advanced SQL-based data manipulation
4. **Deno Runtime**: Secure JavaScript/TypeScript execution environment
5. **SQLite Database**: Local data storage and querying
6. **SQLpage UI**: Browser-based verification and visualization

## 📋 Prerequisites

### Required Software

| Tool | Version | Purpose |
|------|---------|---------|
| [Deno](https://deno.land/) | 2.0+ | TypeScript/JavaScript runtime |
| [surveilr](https://surveilr.com) | Latest | Data processing engine |

### System Requirements

- **OS**: Windows 10/11, macOS 10.15+, Linux (Ubuntu 20.04+)
- **RAM**: Minimum 4GB, Recommended 8GB+
- **Storage**: 1GB+ free space for application and data
- **Network**: Optional (for initial setup only)

## 🚀 Installation

### Step 1: Install Deno

**Windows (PowerShell as Administrator):**

```powershell
irm https://deno.land/install.ps1 | iex
```

**macOS/Linux:**

```bash
curl -fsSL https://deno.land/install.sh | sh
```

**Upgrade to Deno 2.0** (if already installed):

```bash
deno upgrade
```

Verify installation:

```bash
deno --version
```

### Step 2: Install surveilr

1. Download the latest release from [Surveilr Releases](https://github.com/surveilr/surveilr/releases)
2. Place the executable in your project folder or system PATH
3. Verify installation:

**Windows (Command Prompt):**

```cmd
surveilr --version
```

**Windows (PowerShell):**

```powershell
.\surveilr --version
```

**macOS/Linux:**

```bash
./surveilr --version
```
