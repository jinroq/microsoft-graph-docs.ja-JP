---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: fba5222968d25e04bd53e804fe520a742dbda154
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34448655"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var messageRules = await graphClient.Me.MailFolders["inbox"].MessageRules
    .Request()
    .GetAsync();

```