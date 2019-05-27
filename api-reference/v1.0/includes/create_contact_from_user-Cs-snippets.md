---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: cd70bdb94027d811395ee4877f513f55d6cd09d0
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34478476"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contact = new Contact
{
    GivenName = "Pavel",
    Surname = "Bansky",
    EmailAddresses = new List<EmailAddress>()
    {
        new EmailAddress
        {
            Address = "pavelb@fabrikam.onmicrosoft.com",
            Name = "Pavel Bansky"
        }
    },
    BusinessPhones = new List<String>()
    {
        "+1 732 555 0102"
    }
};

await graphClient.Me.Contacts
    .Request()
    .AddAsync(contact);

```