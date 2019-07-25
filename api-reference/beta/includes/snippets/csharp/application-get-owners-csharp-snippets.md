---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d16f0492ac0fd46779bb22045a2f254c6baaa1fa
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35855266"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var owners = await graphClient.Applications["{id}"].Owners
    .Request()
    .GetAsync();

```