---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 5b4cb6792b9ca292b93147729a3c404daabfbd9f
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35728781"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var id = "id-value";

var groupId = "groupId-value";

await graphClient.Me.Onenote.Pages["{id}"]
    .CopyToSection(id,groupId,siteCollectionId,siteId)
    .Request()
    .PostAsync();

```