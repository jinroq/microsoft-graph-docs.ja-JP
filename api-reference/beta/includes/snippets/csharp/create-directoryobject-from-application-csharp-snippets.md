---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 74971536a4712929c2338605a4baa59de23283ba
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/30/2019
ms.locfileid: "35930454"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = new DirectoryObject
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.id","https://graph.microsoft.com/beta/directoryObjects/{id}"}
    }
};

await graphClient.Applications["{id}"].Owners.References
    .Request()
    .AddAsync(directoryObject);

```