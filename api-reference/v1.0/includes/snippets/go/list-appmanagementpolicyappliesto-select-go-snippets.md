---
description: "Automatically generated file. DO NOT MODIFY"
---

```go


import (
	  "context"
	  msgraphsdk "github.com/microsoftgraph/msgraph-sdk-go"
	  graphconfig "github.com/microsoftgraph/msgraph-sdk-go/policies"
	  //other-imports
)

graphClient := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)


requestParameters := &graphconfig.PoliciesAppManagementPolicieItemAppliesToRequestBuilderGetQueryParameters{
	Select: [] string {"id","appId","displayName","createdDateTime"},
}
configuration := &graphconfig.PoliciesAppManagementPolicieItemAppliesToRequestBuilderGetRequestConfiguration{
	QueryParameters: requestParameters,
}

result, err := graphClient.Policies().AppManagementPolicies().ByAppManagementPolicieId("appManagementPolicy-id").AppliesTo().Get(context.Background(), configuration)


```