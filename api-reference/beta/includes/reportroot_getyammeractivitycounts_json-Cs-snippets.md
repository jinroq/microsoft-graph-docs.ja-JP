---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: c0cc58c05aee4a7cd0098a5fec79c0987ef0f1a3
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34478924"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getYammerActivityCounts = await graphClient.Reports.GetYammerActivityCounts('D7')
    .Request()
    .GetAsync();

```