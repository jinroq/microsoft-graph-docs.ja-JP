---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 13ecb4ff895ffbef10fd715b269b4437a5ff7450
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35722809"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var conversation = new Conversation
{
    Topic = "New locations for this quarter",
    Threads = new List<ConversationThread>()
    {
        new ConversationThread
        {
            Posts = new List<Post>()
            {
                new Post
                {
                    Body = new ItemBody
                    {
                        ContentType = BodyType.Html,
                        Content = "What do we know so far?"
                    },
                    NewParticipants = new List<Recipient>()
                    {
                        new Recipient
                        {
                            EmailAddress = new EmailAddress
                            {
                                Name = "Adele Vance",
                                Address = "AdeleV@contoso.onmicrosoft.com"
                            }
                        }
                    }
                }
            }
        }
    }
};

await graphClient.Groups["29981b6a-0e57-42dc-94c9-cd24f5306196"].Conversations
    .Request()
    .AddAsync(conversation);

```