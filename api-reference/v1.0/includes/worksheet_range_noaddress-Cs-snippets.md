---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: c9fa85464b632686053f4b95901e37e29948946f
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34466882"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"].Range()
    .Request()
    .GetAsync();

```