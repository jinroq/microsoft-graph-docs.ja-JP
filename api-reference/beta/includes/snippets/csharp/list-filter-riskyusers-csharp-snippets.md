---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 7d64a8b20e9d6be70f8937dc31142a085d4fdee3
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35526496"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var riskyUsers = await graphClient.RiskyUsers
    .Request()
    .Filter("riskLevel eq microsoft.graph.riskLevel'medium'")
    .GetAsync();

```