---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 225977cd90be1c813c8489792b21b01d95008e5b
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35895102"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var childFolders = await graphClient.Me.MailFolders["{id}"].ChildFolders
    .Request()
    .GetAsync();

```