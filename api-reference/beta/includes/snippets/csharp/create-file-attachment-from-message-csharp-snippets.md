---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 84dcfd5f8135c1b7547431794168ee1e7fd075b2
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35879531"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attachment = new Attachment
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.type","#microsoft.graph.fileAttachment"}
    },
    Name = "smile",
    ContentBytes = "a0b1c76de9f7="
};

await graphClient.Me.Messages["AAMkpsDRVK"].Attachments
    .Request()
    .AddAsync(attachment);

```