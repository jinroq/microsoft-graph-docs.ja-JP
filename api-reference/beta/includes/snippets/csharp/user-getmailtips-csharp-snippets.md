---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: c4fadabb3b5c9bd95bef6475abad4cbdbbd27018
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35527692"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var emailAddresses = new List<String>()
{
    "danas@contoso.onmicrosoft.com",
    "fannyd@contoso.onmicrosoft.com"
};

var mailTipsOptions = MailTipsType.AutomaticReplies | MailTipsType.MailboxFullStatus;

await graphClient.Me
    .GetMailTips(emailAddresses,mailTipsOptions)
    .Request()
    .PostAsync();

```