---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 3a70cf60f3e191faecfebd958f87c90b42e95f55
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35486635"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var chatMessage = await graphClient.Teams["{id}"].Channels["{id}"].Messages["{id}"]
    .Request()
    .GetAsync();

```