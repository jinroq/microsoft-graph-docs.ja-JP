---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: b347e434bf3500bcc418965cef5de340baf71a3d
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34444595"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groupId = "ffffffff-ffff-ffff-ffff-ffffffffffff";

await graphClient.GroupLifecyclePolicies
    .RenewGroup(groupId)
    .Request()
    .PostAsync();

```