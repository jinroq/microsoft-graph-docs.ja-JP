---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 151e1fcdf351275847434e0e5f27b23897fd5ef5
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34469070"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetYammerActivityUserDetail('D7')
    .Request()
    .GetAsync();

```