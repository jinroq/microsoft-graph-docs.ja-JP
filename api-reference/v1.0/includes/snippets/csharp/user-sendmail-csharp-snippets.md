---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 700bce7b4a331c6072582ddd9a8ca3c479decbf4
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35711414"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = new Message
{
    Subject = "Meet for lunch?",
    Body = new ItemBody
    {
        ContentType = BodyType.Text,
        Content = "The new cafeteria is open."
    },
    ToRecipients = new List<Recipient>()
    {
        new Recipient
        {
            EmailAddress = new EmailAddress
            {
                Address = "fannyd@contoso.onmicrosoft.com"
            }
        }
    },
    CcRecipients = new List<Recipient>()
    {
        new Recipient
        {
            EmailAddress = new EmailAddress
            {
                Address = "danas@contoso.onmicrosoft.com"
            }
        }
    }
};

var saveToSentItems = false;

await graphClient.Me
    .SendMail(message,saveToSentItems)
    .Request()
    .PostAsync();

```