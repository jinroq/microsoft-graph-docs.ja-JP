---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 31a5aad70a095546c8ae12f17ec00503da8e2325
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35725738"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var history = await graphClient.RiskyUsers["41a31b00-3b3b-42d9-8f1c-6d4f14e74c69"].History
    .Request()
    .GetAsync();

```