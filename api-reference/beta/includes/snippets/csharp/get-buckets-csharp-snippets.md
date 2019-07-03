---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 9126fec0749cf8b3dd143b11d2b63b59596d3833
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35504025"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var buckets = await graphClient.Planner.Plans["2txjA-BMZEq-bKi6Wfj5aGQAB1OJ"].Buckets
    .Request()
    .GetAsync();

```