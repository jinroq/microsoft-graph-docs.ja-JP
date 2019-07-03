---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 9c5aca27fa617fe465b2eb63e14635906f807203
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35526256"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var clientContext = "clientContext-value";

await graphClient.App.Calls["{id}"]
    .Mute(clientContext)
    .Request()
    .PostAsync();

```