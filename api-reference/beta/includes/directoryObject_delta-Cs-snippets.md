---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: fd9e920f849acb8299eb59db38d24b66e59e555b
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34437322"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = await graphClient.DirectoryObjects["delta"]
    .Request()
    .Filter("isOf('Microsoft.Graph.User')+or+isOf('Microsoft.Graph.Group')")
    .GetAsync();

```