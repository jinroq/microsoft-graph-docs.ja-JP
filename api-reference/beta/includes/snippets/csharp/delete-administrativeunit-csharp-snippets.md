---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 074ce25940385710ff923c1f87555a1fef44262e
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35464455"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.AdministrativeUnits["{id}"]
    .Request()
    .DeleteAsync();

```