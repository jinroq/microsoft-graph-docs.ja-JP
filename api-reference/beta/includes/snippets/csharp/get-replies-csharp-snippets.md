---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 8525273f3ec881b6b1e3003819ed5894c9bd589c
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35707657"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var replies = await graphClient.Chats["{id}"].Messages["{id}"].Replies
    .Request()
    .GetAsync();

```