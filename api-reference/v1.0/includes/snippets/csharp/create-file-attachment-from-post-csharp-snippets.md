---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 2d3bb8ba05dab7d20f4d9d55e4ee7f168a1688b1
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35739628"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attachment = new Attachment
{
    Name = "name-value",
    ContentBytes = "base64-contentBytes-value"
};

await graphClient.Groups["{id}"].Threads["{id}"].Posts["{id}"].Attachments
    .Request()
    .AddAsync(attachment);

```