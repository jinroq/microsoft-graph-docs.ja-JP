---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 69762d057c18edc282cd217fca59d9610362d806
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34456572"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var calculationType = "calculationType-value";

await graphClient.Me.Drive.Items["{id}"].Workbook.Application
    .Calculate(calculationType)
    .Request()
    .PostAsync();

```