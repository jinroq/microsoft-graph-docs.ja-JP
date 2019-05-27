---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: c52999d92ffd7048080e0381185e3a63aec49e2d
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34480667"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var group = new Group
{
    Description = "Self help community for golf",
    DisplayName = "Golf Assist",
    GroupTypes = new List<String>()
    {
        "Unified"
    },
    MailEnabled = true,
    MailNickname = "golfassist",
    SecurityEnabled = false
};

await graphClient.Groups
    .Request()
    .AddAsync(group);

```