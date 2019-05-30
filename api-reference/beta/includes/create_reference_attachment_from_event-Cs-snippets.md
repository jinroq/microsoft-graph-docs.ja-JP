---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: aea6ee894134ff4f14418367836965c391f4dd14
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/29/2019
ms.locfileid: "34546813"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attachment = new Attachment
{
    Name = "Personal pictures",
    SourceUrl = "https://contoso.com/personal/mario_contoso_net/Documents/Pics",
    ProviderType = "oneDriveConsumer",
    Permission = "Edit",
    IsFolder = "True"
};

await graphClient.Me.Events["AAMkAGE1M88AADUv0uAAAG="].Attachments
    .Request()
    .AddAsync(attachment);

```