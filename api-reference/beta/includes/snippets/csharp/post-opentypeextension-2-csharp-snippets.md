---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 9c4c716f177875ce7a5a390c35e05a239a83cedd
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35878418"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var extension = new Extension
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.type","microsoft.graph.openTypeExtension"}
    },
    ExtensionName = "Com.Contoso.Referral",
    CompanyName = "Wingtip Toys",
    DealValue = 500050,
    ExpirationDate = "2015-12-03T10:00:00Z"
};

await graphClient.Me.Messages["AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl==="].Extensions
    .Request()
    .AddAsync(extension);

```