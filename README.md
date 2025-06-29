# Process of getting Azure Credentials

### Download Azure Cli

### open Termainal

```
az login
```
### Get Subscribption ID

```
az account show --query id -o tsv
```

```
az ad sp create-for-rbac --name adf-github-sp --role Contributor --scopes /subscriptions/YOUR_SUBSCRIPTION_ID --sdk-auth
```
