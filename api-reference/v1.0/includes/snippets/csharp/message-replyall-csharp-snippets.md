---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 14c5c1e6d7860a659ffbbf99e2c0f5459e27cbb1
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35731970"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var comment = "comment-value";

await graphClient.Me.Messages["{id}"]
    .ReplyAll(comment)
    .Request()
    .PostAsync();

```