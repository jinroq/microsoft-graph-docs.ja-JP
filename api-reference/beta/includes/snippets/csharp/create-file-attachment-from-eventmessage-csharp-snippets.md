---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6a500e4d5d77f83d2bcaf6d71884a6872b0e6022
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35859351"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attachment = new Attachment
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.type","#Microsoft.OutlookServices.FileAttachment"}
    },
    Name = "name-value",
    ContentType = "contentType-value",
    IsInline = false,
    ContentLocation = "contentLocation-value",
    ContentBytes = "contentBytes-value"
};

await graphClient.Me.Messages["{id}"].Attachments
    .Request()
    .AddAsync(attachment);

```