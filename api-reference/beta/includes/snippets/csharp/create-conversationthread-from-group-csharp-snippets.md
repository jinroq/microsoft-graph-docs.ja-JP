---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 4a729ff4c5d444c90fc21d49acb88542d080f333
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35713515"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var conversationThread = new ConversationThread
{
    Topic = "New Conversation Thread Topic",
    Posts = new List<Post>()
    {
        new Post
        {
            Body = new ItemBody
            {
                ContentType = BodyType.Html,
                Content = "this is body content"
            },
            NewParticipants = new List<Recipient>()
            {
                new Recipient
                {
                    EmailAddress = new EmailAddress
                    {
                        Name = "Alex Darrow",
                        Address = "alexd@contoso.com"
                    }
                }
            }
        }
    }
};

await graphClient.Groups["{id}"].Threads
    .Request()
    .AddAsync(conversationThread);

```