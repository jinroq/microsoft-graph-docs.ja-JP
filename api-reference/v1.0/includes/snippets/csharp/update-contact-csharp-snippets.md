---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: e23c1902299b93cb9bd257c3204d21bec6de79c2
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35741027"
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
    Birthday = "1974-07-22"
};

await graphClient.Me.Contacts["{id}"]
    .Request()
    .UpdateAsync(contact);

```