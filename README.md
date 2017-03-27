# Media Forensics Using Azure Cognitive Services

This [Azure Function](https://docs.microsoft.com/en-us/azure/azure-functions/functions-overview) will process images using the 
[Azure Cognitive Services Computer Vision](https://www.microsoft.com/cognitive-services/en-us/computer-vision-api), transcribe text from audio WAV files using the 
[Azure Cognitive Services Bing Speech API](https://www.microsoft.com/cognitive-services/en-us/speech-api) and perform text analysis on the transcribed text using 
the [Azure Cognitive Services Text Analysis API](https://www.microsoft.com/cognitive-services/en-us/speech-api)


## What you'll need

- An [Azure Subscription](https://azure.microsoft.com/en-gb/free/?&WT.srch=1&WT.mc_ID=SEM_Bing_UKAzureBG_)
- An [Azure Function App](https://docs.microsoft.com/en-us/azure/azure-functions/functions-overview)
- An [Azure DocumentDB](https://azure.microsoft.com/en-us/services/documentdb/) instance
- An [Azure Storage Account](https://azure.microsoft.com/en-gb/services/storage/)


To make this demo work, you need to clone or download this repository, then - 

### Edit the appsettings.json files with your own values

```javascript
{
  "IsEncrypted": false,
  "Values": {
    "AzureWebJobsStorage": "DefaultEndpointsProtocol=https;AccountName=[StorageAccountName];AccountKey=[Storage Account Key];",
    "AzureWebJobsDashboard": "DefaultEndpointsProtocol=https;AccountName=[StorageAccountName];AccountKey=[Storage Account Key];",
    "DocumentDBConnection": "AccountEndpoint=[Document DB EndPoint];AccountKey=[Document DB Account Key];"
	"ComputerVisionSubscriptionKey": "[Your Cognitive Services Computer Vision Key]"
  }
}
```



### Upload the Functions code to you Azure Function App Environment
- You can do this in Visual Studio by right clicking on the project name and selecting 'Deploy'.
- You can use [Continuous Integration](https://docs.microsoft.com/en-us/azure/azure-functions/functions-continuous-deployment)
- Cut and paste this code into [a Function you created in the Azure Portal](https://docs.microsoft.com/en-us/azure/azure-functions/functions-create-first-azure-function-azure-portal)



## Learn more about developing [Azure Functions](https://docs.microsoft.com/en-us/azure/azure-functions/functions-reference)


