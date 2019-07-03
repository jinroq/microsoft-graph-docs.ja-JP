---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 8525273f3ec881b6b1e3003819ed5894c9bd589c
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35527194"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var replies = await graphClient.Chats["{id}"].Messages["{id}"].Replies
    .Request()
    .GetAsync();

```