---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: f7b26893333fb502127daf0440e51a5e0efe44ff
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34436384"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var Call = await graphClient.App.Calls["{id}"]
    .Request()
    .GetAsync();

```