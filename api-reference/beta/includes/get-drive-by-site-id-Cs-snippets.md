---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: fdcafc495087b78ccc156b4fe25fdcca7b97636d
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34483276"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var drive = await graphClient.Sites["{siteId}"].Drive
    .Request()
    .GetAsync();

```