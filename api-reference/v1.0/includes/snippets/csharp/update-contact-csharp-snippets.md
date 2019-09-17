---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 369396d02b2335a19438be2e9565b44950744ae3
ms.sourcegitcommit: d8a58221ed1f2b7b7073fd621da4737e11ba53c5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/11/2019
ms.locfileid: "36846147"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contact = new Contact
{
    HomeAddress = new PhysicalAddress
    {
        Street = "123 Some street",
        City = "Seattle",
        State = "WA",
        PostalCode = "98121"
    },
    Birthday = DateTimeOffset.Parse("1974-07-22")
};

await graphClient.Me.Contacts["{id}"]
    .Request()
    .UpdateAsync(contact);

```