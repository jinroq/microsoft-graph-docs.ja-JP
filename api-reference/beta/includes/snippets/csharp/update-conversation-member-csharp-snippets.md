---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 7a3ed4c4edf66da464d64bd5728fab2e2b47e217
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/27/2019
ms.locfileid: "36634008"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var conversationMember = new ConversationMember
{
    Roles = new List<String>()
    {
        "owner"
    }
};

await graphClient.Teams["{id}"].Channels["{id}"].Members["{id}"]
    .Request()
    .UpdateAsync(conversationMember);

```