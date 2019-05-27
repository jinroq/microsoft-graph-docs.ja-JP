---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 43c63a9b10f7e1c08d25dd68241af07a30d20930
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34469449"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groupIds = new List<String>()
{
    "groupIds-value"
};

await graphClient.ServicePrincipals["{id}"]
    .CheckMemberGroups(groupIds)
    .Request()
    .PostAsync();

```