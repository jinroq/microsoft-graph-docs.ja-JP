---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: c575ccd60a5c548dee2cfca68570c74c86c4ae06
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34449147"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var me = await graphClient.Me
    .Request()
    .Select( e => new {
             e.MailboxSettings 
             })
    .GetAsync();

var mailboxSettings = me.MailboxSettings;

```