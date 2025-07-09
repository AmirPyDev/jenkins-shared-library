# Jenkins Shared Library Example

This repository is a template for a Jenkins Shared Library written in Groovy.

## Directory Structure
- `vars/` — Global variables (steps) accessible in Jenkins pipelines.
- `src/` — Groovy classes for advanced logic.
- `resources/` — Non-Groovy resources (e.g., templates).

## Usage
1. Place this repository in your SCM (e.g., GitHub).
2. In your Jenkins pipeline, load the library:
   ```groovy
   @Library('your-shared-library') _
   customStep('Jenkins User')
   ```
3. Add more steps in `vars/` or classes in `src/` as needed.

## Example Step
See `vars/customStep.groovy` for a sample step.

---
For more information, see the [Jenkins Shared Library documentation](https://www.jenkins.io/doc/book/pipeline/shared-libraries/).
