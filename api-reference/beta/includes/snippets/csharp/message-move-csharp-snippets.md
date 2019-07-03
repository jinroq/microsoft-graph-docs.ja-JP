---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 3746628347e22d4c4bb86cf57367dc04b212bb59
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35485260"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var destinationId = "deleteditems";

await graphClient.Me.Messages["AAMkADhAAATs28OAAA="]
    .Move(destinationId)
    .Request()
    .PostAsync();

```