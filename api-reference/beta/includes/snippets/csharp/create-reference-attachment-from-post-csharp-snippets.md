---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: e19715bd9090cc38f0fcb746387a861f8b39de52
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/27/2019
ms.locfileid: "36634022"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attachment = new Attachment
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.type","#microsoft.graph.referenceAttachment"}
    },
    Name = "Personal pictures",
    SourceUrl = "https://contoso.com/personal/mario_contoso_net/Documents/Pics",
    ProviderType = "oneDriveConsumer",
    Permission = "Edit",
    IsFolder = "True"
};

await graphClient.Groups["c75831bdfad"].Threads["AAQkAGF97XEKhULw"].Posts["AAMkAGFcAAA"].Attachments
    .Request()
    .AddAsync(attachment);

```