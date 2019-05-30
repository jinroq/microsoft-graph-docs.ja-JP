---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 5c1d56ef7984f720e63c6c8ad904682b4ab1e809
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/29/2019
ms.locfileid: "34546811"
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

await graphClient.Me.Messages["AAMkAGE1M88AADUv0uFAAA="].Attachments
    .Request()
    .AddAsync(attachment);

```