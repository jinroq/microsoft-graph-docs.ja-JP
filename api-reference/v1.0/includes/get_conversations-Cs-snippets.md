---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: b60d6146a22b612e7f1093ad1dbdbc6ca304fec4
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34467449"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var conversations = await graphClient.Groups["{id}"].Conversations
    .Request()
    .GetAsync();

```