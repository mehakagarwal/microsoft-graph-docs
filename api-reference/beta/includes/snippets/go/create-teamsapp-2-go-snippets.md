---
description: "Automatically generated file. DO NOT MODIFY"
---

```go


import (
	  "context"
	  msgraphsdk "github.com/microsoftgraph/msgraph-beta-sdk-go"
	  graphconfig "github.com/microsoftgraph/msgraph-beta-sdk-go/appcatalogs"
	  //other-imports
)

graphClient := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)



requestRequiresreview := true

requestParameters := &graphconfig.AppCatalogsTeamsAppsRequestBuilderPostQueryParameters{
	Requiresreview: &requestRequiresreview,
}
configuration := &graphconfig.AppCatalogsTeamsAppsRequestBuilderPostRequestConfiguration{
	QueryParameters: requestParameters,
}

graphClient.AppCatalogs().TeamsApps().Post(context.Background(), configuration)


```