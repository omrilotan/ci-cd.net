---
title: Hosted CI/CD scripts
toc: true
---

A collection of hosted CI-CD generic helper scripts, which aim to streamline continues integration and delivery processes across services. This project's goal is to include non business logic scripts which can be used out-of-the-box or adapted by arguments.

## Using hosted shell scripts
Using a script with defaults
```
curl ci-cd.net/v1/<SCRIPT> | sh
```

Passing arguments
```bash
curl ci-cd.net/v1/<SCRIPT> | sh -s <ARGUMENT_1> <ARGUMENT_2>
```
