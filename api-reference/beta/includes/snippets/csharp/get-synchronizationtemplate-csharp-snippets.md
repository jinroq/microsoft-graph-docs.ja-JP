---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 957b0e8db1a6c2094b3b51b04bd043cee6f15d56
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35527161"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var templates = await graphClient.ServicePrincipals["{id}"].Synchronization.Templates
    .Request()
    .GetAsync();

```