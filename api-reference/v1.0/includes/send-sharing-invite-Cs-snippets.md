---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 4ea96b5fa293aef934a5062eeb57466868c123da
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34455829"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var recipients = new List<DriveRecipient>()
{
    new DriveRecipient
    {
        Email = "ryan@contoso.com"
    }
};

var message = "Here's the file that we're collaborating on.";

var requireSignIn = true;

var sendInvitation = true;

var roles = new List<String>()
{
    "write"
};

await graphClient.Me.Drive.Items["{item-id}"]
    .Invite(requireSignIn,roles,sendInvitation,message,recipients)
    .Request()
    .PostAsync();

```