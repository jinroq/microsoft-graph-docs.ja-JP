---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: b893b6519c45e1dc5269f34173c9ed13bcf999d7
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35724304"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var me = await graphClient.Me
    .Request()
    .Select( e => new {
             e.MailboxSettings 
             })
    .GetAsync();

var automaticRepliesSetting = me.MailboxSettings.AutomaticRepliesSetting;

```