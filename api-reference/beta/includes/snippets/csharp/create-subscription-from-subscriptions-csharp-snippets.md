---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 08521386009ab8256769acec0ce4684cf2be371a
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35717451"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var subscription = new Subscription
{
    ChangeType = "created,updated",
    NotificationUrl = "https://webhook.azurewebsites.net/api/send/myNotifyClient",
    Resource = "me/mailFolders('Inbox')/messages",
    ExpirationDateTime = "2016-11-20T18:23:45.9356913Z",
    ClientState = "secretClientValue"
};

await graphClient.Subscriptions
    .Request()
    .AddAsync(subscription);

```