---
description: "Automatically generated file. DO NOT MODIFY"
---

```go


// Code snippets are only available for the latest major version. Current major version is $v1.*

// Dependencies
import (
	  "context"
	  msgraphsdk "github.com/microsoftgraph/msgraph-sdk-go"
	  graphmodels "github.com/microsoftgraph/msgraph-sdk-go/models"
	  //other-imports
)

requestBody := graphmodels.NewDeviceConfiguration()
description := "Description value"
requestBody.SetDescription(&description) 
displayName := "Display Name value"
requestBody.SetDisplayName(&displayName) 
version := int32(7)
requestBody.SetVersion(&version) 
accountManagerPolicy := graphmodels.NewSharedPCAccountManagerPolicy()
accountDeletionPolicy := graphmodels.DISKSPACETHRESHOLD_SHAREDPCACCOUNTDELETIONPOLICYTYPE 
accountManagerPolicy.SetAccountDeletionPolicy(&accountDeletionPolicy) 
cacheAccountsAboveDiskFreePercentage := int32(4)
accountManagerPolicy.SetCacheAccountsAboveDiskFreePercentage(&cacheAccountsAboveDiskFreePercentage) 
inactiveThresholdDays := int32(5)
accountManagerPolicy.SetInactiveThresholdDays(&inactiveThresholdDays) 
removeAccountsBelowDiskFreePercentage := int32(5)
accountManagerPolicy.SetRemoveAccountsBelowDiskFreePercentage(&removeAccountsBelowDiskFreePercentage) 
requestBody.SetAccountManagerPolicy(accountManagerPolicy)
allowedAccounts := graphmodels.DOMAIN_SHAREDPCALLOWEDACCOUNTTYPE 
requestBody.SetAllowedAccounts(&allowedAccounts) 
allowLocalStorage := true
requestBody.SetAllowLocalStorage(&allowLocalStorage) 
disableAccountManager := true
requestBody.SetDisableAccountManager(&disableAccountManager) 
disableEduPolicies := true
requestBody.SetDisableEduPolicies(&disableEduPolicies) 
disablePowerPolicies := true
requestBody.SetDisablePowerPolicies(&disablePowerPolicies) 
disableSignInOnResume := true
requestBody.SetDisableSignInOnResume(&disableSignInOnResume) 
enabled := true
requestBody.SetEnabled(&enabled) 
idleTimeBeforeSleepInSeconds := int32(12)
requestBody.SetIdleTimeBeforeSleepInSeconds(&idleTimeBeforeSleepInSeconds) 
kioskAppDisplayName := "Kiosk App Display Name value"
requestBody.SetKioskAppDisplayName(&kioskAppDisplayName) 
kioskAppUserModelId := "Kiosk App User Model Id value"
requestBody.SetKioskAppUserModelId(&kioskAppUserModelId) 
maintenanceStartTime := 11:59:24.7240000
requestBody.SetMaintenanceStartTime(&maintenanceStartTime) 

// To initialize your graphClient, see https://learn.microsoft.com/en-us/graph/sdks/create-client?from=snippets&tabs=go
deviceConfigurations, err := graphClient.DeviceManagement().DeviceConfigurations().Post(context.Background(), requestBody, nil)


```