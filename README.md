# Kotlin Workflows

## Overview

This repository contains reusable GitHub Actions workflows tailored for Kotlin projects. These workflows are designed to be shared across multiple repositories within the organization to ensure consistency, reduce duplication, and simplify CI/CD pipeline maintenance.

Currently, the workflows focus on building and testing Kotlin applications using Gradle.

## Workflows

### `build.yml`

- **Purpose:** Builds the Kotlin project and runs tests using Gradle.
- **Trigger:** Designed to be called as a reusable workflow (`workflow_call`) from other repositories.
- **Inputs:**
    - `kotlin-version` (optional): Specifies the JDK version to use for the build. Defaults to `1.8`.
- **Jobs:**
    - Checks out the code.
    - Sets up the Java environment with the specified Kotlin/JDK version.
    - Runs the Gradle build and tests.

---

Feel free to contribute by adding new workflows or improving existing ones to support other Kotlin-related CI/CD tasks.
