---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 1325b661d7b5907d33eaab7f326ca01e64402620
ms.sourcegitcommit: d8a58221ed1f2b7b7073fd621da4737e11ba53c5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/11/2019
ms.locfileid: "36846124"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var value = new List<TiIndicator>()
{
    new TiIndicator
    {
        ActivityGroupNames = new List<String>()
        {
        },
        Confidence = 0,
        Description = "This is a canary indicator for demo purpose. Take no action on any observables set in this indicator.",
        ExpirationDateTime = DateTimeOffset.Parse("2019-03-01T21:44:03.1668987+00:00"),
        ExternalId = "Test--8586509942423126760MS164-0",
        FileHashType = FileHashType.Sha256,
        FileHashValue = "b555c45c5b1b01304217e72118d6ca1b14b7013644a078273cea27bbdc1cf9d6",
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
    },
    new TiIndicator
    {
        ActivityGroupNames = new List<String>()
        {
        },
        Confidence = 0,
        Description = "This is a canary indicator for demo purpose. Take no action on any observables set in this indicator.",
        ExpirationDateTime = DateTimeOffset.Parse("2019-03-01T21:44:03.1748779+00:00"),
        ExternalId = "Test--8586509942423126760MS164-1",
        FileHashType = FileHashType.Sha256,
        FileHashValue = "1796b433950990b28d6a22456c9d2b58ced1bdfcdf5f16f7e39d6b9bdca4213b",
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
    }
};

await graphClient.Security.TiIndicators
    .SubmitTiIndicators(value)
    .Request()
    .PostAsync();

```