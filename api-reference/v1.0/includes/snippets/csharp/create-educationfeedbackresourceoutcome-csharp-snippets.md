---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

// Code snippets are only available for the latest version. Current version is 5.x

var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new EducationOutcome
{
	OdataType = "#microsoft.graph.educationFeedbackResourceOutcome",
	AdditionalData = new Dictionary<string, object>
	{
		{
			"feedbackResource" , new 
			{
				OdataType = "#microsoft.graph.educationWordResource",
				DisplayName = "Document1.docx",
			}
		},
	},
};
var result = await graphClient.Education.Classes["{educationClass-id}"].Assignments["{educationAssignment-id}"].Submissions["{educationSubmission-id}"].Outcomes.PostAsync(requestBody);


```