---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: f89534bffeff6c7b12391d7a97b8715cb110b34e
ms.sourcegitcommit: d8a58221ed1f2b7b7073fd621da4737e11ba53c5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/11/2019
ms.locfileid: "36846111"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var callbackUri = "callbackUri-value";

var mediaConfig = new MediaConfig
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.type","#microsoft.graph.appHostedMediaConfig"}
    },
    Blob = "<media config blob>"
};

var acceptedModalities = new List<Modality>()
{
    Modality.Audio
};

await graphClient.App.Calls["{id}"]
    .Answer(callbackUri,mediaConfig,acceptedModalities)
    .Request()
    .PostAsync();

```