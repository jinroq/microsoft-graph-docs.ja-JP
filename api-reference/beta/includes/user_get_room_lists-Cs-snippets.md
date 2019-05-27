---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: b26c76d2aa31188f948665765326b3de612540dc
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34450392"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var findRoomLists = await graphClient.Me.FindRoomLists()
    .Request()
    .GetAsync();

```