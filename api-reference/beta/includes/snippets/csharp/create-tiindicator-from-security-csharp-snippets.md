---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 9f8a4f2c5812154aa5cc9bbd7829996a6346393d
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35716862"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tiIndicator = new TiIndicator
{
    Action = TiAction.Alert,
    ActivityGroupNames = new List<String>()
    {
    },
    Confidence = 0,
    Description = "This is a canary indicator for demo purpose. Take no action on any observables set in this indicator.",
    ExpirationDateTime = "2019-03-02T00:43:37.5031462+03:00",
    ExternalId = "Test--8586509942679764298MS501",
    FileHashType = FileHashType.Sha256,
    FileHashValue = "aa64428647b57bf51524d1756b2ed746e5a3f31b67cf7fe5b5d8a9daf07ca313",
    KillChain = new List<String>()
    {
    },
    MalwareFamilyNames = new List<String>()
    {
    },
    Severity = 0,
    Tags = new List<String>()
    {
    },
    TargetProduct = "Azure Sentinel",
    ThreatType = "WatchList",
    TlpLevel = TlpLevel.Green
};

await graphClient.Security.TiIndicators
    .Request()
    .AddAsync(tiIndicator);

```