---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 745fb5db33464d41117664b7dd30123d49c6c5d2
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35471109"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerBucket = await graphClient.Planner.Buckets["{bucket-id}"]
    .Request()
    .GetAsync();

```