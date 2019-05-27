---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 9f8964b5fcb0f1d2b93591cdff6f68400a0199ed
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34435614"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var posts = await graphClient.Groups["{id}"].Threads["{id}"].Posts
    .Request()
    .GetAsync();

```