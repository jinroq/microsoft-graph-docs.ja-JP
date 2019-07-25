---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 511ca9cc317bc26c1ba68bb5332366d7abd452bc
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35859651"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Recipient> toRecipientsList = new LinkedList<Recipient>();
Recipient toRecipients = new Recipient();
EmailAddress emailAddress = new EmailAddress();
emailAddress.address = "danas@contoso.onmicrosoft.com";
emailAddress.name = "Dana Swope";
toRecipients.emailAddress = emailAddress;

toRecipientsList.add(toRecipients);

String comment = "Dana, hope you can make this meeting.";

graphClient.me().events("{id}")
    .forward(comment,toRecipientsList)
    .buildRequest()
    .post();

```