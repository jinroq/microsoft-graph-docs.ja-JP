---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6a27aa30b8d48cd6a7c79bbcf4224440dcdd15b2
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35485343"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var callbackUri = "callbackUri-value";

var mediaConfig = new MediaConfig
{
    Blob = "<media config blob>"
};

var acceptedModalities = new List<String>()
{
    "audio"
};

await graphClient.App.Calls["{id}"]
    .Answer(callbackUri,mediaConfig,acceptedModalities)
    .Request()
    .PostAsync();

```