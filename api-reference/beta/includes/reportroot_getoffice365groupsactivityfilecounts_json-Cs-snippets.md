---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 0f6bc876ea323c317577aee9eab5448ebe04e693
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34441431"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getOffice365GroupsActivityFileCounts = await graphClient.Reports.GetOffice365GroupsActivityFileCounts('D7')
    .Request()
    .GetAsync();

```