---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d3460289049e51b40b6b03984ddc6a8db7a0d335
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35472412"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{id}"].Workbook
    .CloseSession(this)
    .Request()
    .Header("workbook-session-id","{session-id}")
    .PostAsync();

```