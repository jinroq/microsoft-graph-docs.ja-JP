---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 9126fec0749cf8b3dd143b11d2b63b59596d3833
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35720537"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var buckets = await graphClient.Planner.Plans["2txjA-BMZEq-bKi6Wfj5aGQAB1OJ"].Buckets
    .Request()
    .GetAsync();

```