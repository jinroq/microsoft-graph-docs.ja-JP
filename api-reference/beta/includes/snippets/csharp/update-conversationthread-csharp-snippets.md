---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 7054feb5a7b1d1ddb6f2f2d401ef164cdfe7c150
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35526557"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var conversationThread = new ConversationThread
{
    IsLocked = true
};

await graphClient.Groups["{id}"].Threads["{id}"]
    .Request()
    .UpdateAsync(conversationThread);

```