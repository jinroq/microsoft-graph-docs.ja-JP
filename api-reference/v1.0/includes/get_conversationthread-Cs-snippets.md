---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: abbfb091f6ec6725e544267d46af2e1b06015d90
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34467435"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var conversationThread = await graphClient.Groups["{id}"].Threads["{id}"]
    .Request()
    .GetAsync();

```