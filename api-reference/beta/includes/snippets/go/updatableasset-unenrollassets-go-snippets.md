---
description: "Automatically generated file. DO NOT MODIFY"
---

```go


import (
	  "context"
	  msgraphsdk "github.com/microsoftgraph/msgraph-beta-sdk-go"
	  graphmodels "github.com/microsoftgraph/msgraph-beta-sdk-go/Admin/Windows/Updates/UpdatableAssets/MicrosoftGraphWindowsUpdatesUnenrollAssets"
	  //other-imports
)

graphClient := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)


requestBody := graphmodels.NewUnenrollAssetsPostRequestBody()
updateCategory := graphmodels.STRING_UPDATECATEGORY 
requestBody.SetUpdateCategory(&updateCategory) 


updatableAsset := graphmodels.NewUpdatableAsset()
id := "String (identifier)"
updatableAsset.SetId(&id) 

assets := []graphmodels.Objectable {
	updatableAsset,

}
requestBody.SetAssets(assets)

graphClient.Admin().Windows().Updates().UpdatableAssets().MicrosoftGraphWindowsUpdatesUnenrollAssets().Post(context.Background(), requestBody, nil)


```