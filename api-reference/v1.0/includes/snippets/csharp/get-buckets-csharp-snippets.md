---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 9c80211545ca96b6afd85c4b89e2894dff26ec13
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35733279"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var buckets = await graphClient.Planner.Plans["{plan-id}"].Buckets
    .Request()
    .GetAsync();

```