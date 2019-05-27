---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d6b6fef0b4ed19651c0f3fad7c659a6e104279aa
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34438155"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.GroupLifecyclePolicies["{id}"]
    .Request()
    .DeleteAsync();

```