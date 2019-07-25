---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a8abced56ccc8bfe3361b006b2457459db0498a8
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35869467"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Subscription subscription = new Subscription();
subscription.changeType = "created,updated";
subscription.notificationUrl = "https://webhook.azurewebsites.net/api/send/myNotifyClient";
subscription.resource = "me/mailFolders('Inbox')/messages";
subscription.expirationDateTime = "2016-11-20T18:23:45.9356913Z";
subscription.clientState = "secretClientValue";

graphClient.subscriptions()
    .buildRequest()
    .post(subscription);

```