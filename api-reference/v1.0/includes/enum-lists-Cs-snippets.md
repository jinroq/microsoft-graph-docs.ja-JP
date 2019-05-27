---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 068f5dbf853313db72b05ec616cc79333ce671dc
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34457931"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var lists = await graphClient.Sites["{site-id}"].Lists
    .Request()
    .GetAsync();

```