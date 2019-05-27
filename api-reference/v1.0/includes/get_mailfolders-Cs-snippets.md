---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 988379b0f1f73bbff16c66dc5df4999258d89eb0
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34477825"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var mailFolders = await graphClient.Me.MailFolders
    .Request()
    .GetAsync();

```