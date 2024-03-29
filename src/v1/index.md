# Hosted CI/CD scripts

A collection of hosted CI-CD generic helper scripts, which aim to streamline continues integration and delivery processes across services. This project's goal is to include non business logic scripts which can be used out-of-the-box or adapted by arguments.

## Using hosted shell scripts
Using a script with defaults
```bash
curl ci-cd.net/v1/<SCRIPT> | bash
```

Passing arguments
```bash
curl ci-cd.net/v1/<SCRIPT> | bash -s <ARGUMENT_1> <ARGUMENT_2>
```

Using SSL
```bash
curl -v https://ci-cd.net/v1/<SCRIPT> | bash
```
