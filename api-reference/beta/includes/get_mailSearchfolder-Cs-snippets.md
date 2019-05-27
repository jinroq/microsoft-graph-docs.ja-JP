---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 05ab5754a0baed2a67836625b8e0c5de10f31786
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34449245"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var mailFolder = await graphClient.Me.MailFolders["AAMkAGVmMDEzN"]
    .Request()
    .GetAsync();

```