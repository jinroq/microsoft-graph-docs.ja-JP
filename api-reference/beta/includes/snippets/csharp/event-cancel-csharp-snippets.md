---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d6fd34cac6e237a97ffc4dc56b72f9e57c9099e9
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35712246"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var comment = "Cancelling for this week due to all hands";

await graphClient.Me.Events["{id}"]
    .Cancel(comment)
    .Request()
    .PostAsync();

```