---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 29efcb266954cb7d3326fc679fb2d6cb9b479173
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/30/2019
ms.locfileid: "35931656"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var recipients = new List<DriveRecipient>()
{
    new DriveRecipient
    {
        Email = "john@contoso.com"
    },
    new DriveRecipient
    {
        Email = "ryan@external.com"
    }
};

var roles = new List<String>()
{
    "read"
};

await graphClient.Shares["{encoded-sharing-url}"].Permission
    .Grant(roles,recipients)
    .Request()
    .PostAsync();

```