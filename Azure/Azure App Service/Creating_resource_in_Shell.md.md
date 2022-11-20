### Creating App service in Powershell

Creating a new resource group

```ps
New-AzResourceGroup 
	-Name "powershellwebapp" 
	-Location "EastUS"
```

Creating app service plan

```ps
New-AzAppServicePlan 
-ResourceGroupName "powershellwebapp" 
-Name "aznewapp123" 
-Location "EastUS" 
-Tier "Free"
```

Creating a web app

```ps
New-AzWebApp -ResourceGroupName "powershellwebapp" -Name "azbalawebapp" -Location "EastUS" -AppServicePlan "aznewapp123"
```

### Creating App service in CLI
Creating a resource group

```bash
az group create --name cliwebapp --location eastus
```

Creating app service plan

```bash
az appservice plan create -g cliwebapp -n mycliwebapp
```

Creating a web app

```bash
az webapp create -g cliwebapp -n balamuruganwebapp -p mycliwebapp
```

### Autodetecting App Service 
The command `up` will autodetect resource groups, appservice plans for a webapp and creates them automatically in a single command
```bash
az webapp up --location eastus --name webapp-bala --html
```