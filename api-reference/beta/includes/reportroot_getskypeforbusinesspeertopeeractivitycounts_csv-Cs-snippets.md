---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 55125a284f587db3f5706bac9cc0a83f34d887b0
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34463926"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getSkypeForBusinessPeerToPeerActivityCounts = await graphClient.Reports.GetSkypeForBusinessPeerToPeerActivityCounts('D7')
    .Request()
    .GetAsync();

```