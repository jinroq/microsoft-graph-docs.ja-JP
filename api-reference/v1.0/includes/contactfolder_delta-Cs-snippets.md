---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: cebc9f1372097ca89c92f16edc9e9061cca9f3c2
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34481759"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Me.ContactFolders.Delta()
    .Request()
    .Header("Prefer","odata.maxpagesize=2")
    .GetAsync();

```