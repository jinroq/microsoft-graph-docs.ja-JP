---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 510ad31949da3e4bb6b29a020083dcd2fd3cd90c
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35526751"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var jobs = await graphClient.ServicePrincipals["{id}"].Synchronization.Jobs
    .Request()
    .GetAsync();

```