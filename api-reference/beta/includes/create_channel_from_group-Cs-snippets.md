---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: cac770ea5ab74c855869e626b57a9828b1205ac5
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34457186"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var channel = new Channel
{
    DisplayName = "Architecture Discussion",
    Description = "This channel is where we debate all future architecture plans"
};

await graphClient.Teams["{id}"].Channels
    .Request()
    .AddAsync(channel);

```