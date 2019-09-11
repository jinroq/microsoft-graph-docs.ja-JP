---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: c5b7cbfcef66100326bea9083bc744ed775c6642
ms.sourcegitcommit: d8a58221ed1f2b7b7073fd621da4737e11ba53c5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/11/2019
ms.locfileid: "36846127"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var subscription = new Subscription
{
    ChangeType = "created,updated",
    NotificationUrl = "https://webhook.azurewebsites.net/api/send/myNotifyClient",
    Resource = "me/mailFolders('Inbox')/messages",
    ExpirationDateTime = DateTimeOffset.Parse("2016-11-20T18:23:45.9356913Z"),
    ClientState = "secretClientValue"
};

await graphClient.Subscriptions
    .Request()
    .AddAsync(subscription);

```