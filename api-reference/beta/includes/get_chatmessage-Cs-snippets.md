---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 3d9429f6e5411bf07d67ab5618ec3e093157833d
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35320283"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var chatMessage = await graphClient.Chats["{id}"].Messages["{id}"]
    .Request()
    .GetAsync();

```