---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 570c13b07cb5a548902e05eef7f6fb63d980c44f
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35862877"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var conversationThread = new ConversationThread
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.type","#Microsoft.OutlookServices.ConversationThread"}
    },
    IsLocked = true
};

await graphClient.Groups["{id}"].Threads["{id}"]
    .Request()
    .UpdateAsync(conversationThread);

```