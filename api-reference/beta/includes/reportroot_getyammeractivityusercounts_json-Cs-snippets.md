---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 8f4f76b3fe770413b516cca0ff20740ceb55256e
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34481724"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getYammerActivityUserCounts = await graphClient.Reports.GetYammerActivityUserCounts('D7')
    .Request()
    .GetAsync();

```