---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: ef871a1fadc96648d89c0c0856c7cdcde582c9b1
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35320023"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var chatMessage = new ChatMessage
{
    Body = new ItemBody
    {
        Content = "Hello world"
    }
};

await graphClient.Teams["{id}"].Channels["{id}"].Messages["{id}"].Replies
    .Request()
    .AddAsync(chatMessage);

```