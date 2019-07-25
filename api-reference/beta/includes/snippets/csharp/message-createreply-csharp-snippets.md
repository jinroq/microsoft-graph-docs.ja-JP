---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 38f6164afc41be8f1724ca48fd2f8c6491edfb0f
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35721517"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = new Message
{
    ToRecipients = new List<Recipient>()
    {
        new Recipient
        {
            EmailAddress = new EmailAddress
            {
                Address = "samanthab@contoso.onmicrosoft.com",
                Name = "Samantha Booth"
            }
        },
        new Recipient
        {
            EmailAddress = new EmailAddress
            {
                Address = "randiw@contoso.onmicrosoft.com",
                Name = "Randi Welch"
            }
        }
    }
};

var comment = "Samantha, Randi, would you name the group if the project is approved, please?";

await graphClient.Me.Messages["AAMkADA1MTAAAAqldOAAA="]
    .CreateReply(message,comment)
    .Request()
    .PostAsync();

```