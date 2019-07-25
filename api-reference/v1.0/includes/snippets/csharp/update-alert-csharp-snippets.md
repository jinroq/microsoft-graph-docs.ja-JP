---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: cad2313629109debe5d0886cccd9f3f21f1fe032
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35733404"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var alert = new Alert
{
    AssignedTo = "String",
    ClosedDateTime = "String (timestamp)",
    Comments = new List<String>()
    {
        "String"
    },
    Feedback = AlertFeedback.Unknown,
    Status = AlertStatus.Unknown,
    Tags = new List<String>()
    {
        "String"
    },
    VendorInformation = new SecurityVendorInformation
    {
        Provider = "String",
        Vendor = "String"
    }
};

await graphClient.Security.Alerts["{alert_id}"]
    .Request()
    .Header("Prefer","return=representation")
    .UpdateAsync(alert);

```