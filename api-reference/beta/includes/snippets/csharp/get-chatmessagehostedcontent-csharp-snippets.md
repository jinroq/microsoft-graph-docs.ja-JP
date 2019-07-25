---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 4a989092aae67a3885a0b27c3fa169c522d618e4
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35707615"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var chatMessageHostedContent = await graphClient.Chats["{id}"].Messages["{id}"].HostedContents["{id}"]
    .Request()
    .GetAsync();

```