---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: f6b000641e6a90f97e1e39b5e8fd956cdf8ddfe2
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35715596"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var conversationThread = new ConversationThread
{
    Topic = "topic-value",
    Posts = new List<Post>()
    {
        new Post
        {
            Body = new ItemBody
            {
                ContentType = BodyType.Html,
                Content = "this is body content"
            }
        }
    }
};

await graphClient.Groups["{id}"].Conversations["{id}"].Threads
    .Request()
    .AddAsync(conversationThread);

```