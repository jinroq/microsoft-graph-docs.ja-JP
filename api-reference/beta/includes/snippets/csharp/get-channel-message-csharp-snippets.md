---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 3a70cf60f3e191faecfebd958f87c90b42e95f55
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35707594"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var chatMessage = await graphClient.Teams["{id}"].Channels["{id}"].Messages["{id}"]
    .Request()
    .GetAsync();

```