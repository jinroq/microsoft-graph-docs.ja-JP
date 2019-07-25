---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: c2e12034899cf64dd9848a8aa3db1b2ec5615311
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35858012"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = new DirectoryObject
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.id","https://graph.microsoft.com/beta/users/{id}"}
    }
};

await graphClient.Groups["{id}"].Owners.References
    .Request()
    .AddAsync(directoryObject);

```