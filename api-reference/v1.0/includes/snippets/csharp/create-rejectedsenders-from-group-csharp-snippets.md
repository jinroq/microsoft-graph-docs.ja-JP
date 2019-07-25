---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 758d8f6aafe07c199a89a7a1742d76f0f30eea41
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35885505"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = new DirectoryObject
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.id","https://graph.microsoft.com/v1.0/users/alexd@contoso.com"}
    }
};

await graphClient.Groups["{id}"].RejectedSenders.References
    .Request()
    .AddAsync(directoryObject);

```