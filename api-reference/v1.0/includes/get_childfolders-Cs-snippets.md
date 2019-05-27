---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 225977cd90be1c813c8489792b21b01d95008e5b
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34467763"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var childFolders = await graphClient.Me.MailFolders["{id}"].ChildFolders
    .Request()
    .GetAsync();

```