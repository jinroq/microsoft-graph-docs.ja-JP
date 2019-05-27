---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 702cd9ecf9e6c1d6279e5308ac5f9e1b003c6a9e
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34480275"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var findRooms = await graphClient.Me.FindRooms()
    .Request()
    .GetAsync();

```