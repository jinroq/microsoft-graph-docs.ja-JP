---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 8b439032b3fdbd83ec6b85793d803656c0acb355
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34441760"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getOffice365ActivationsUserCounts = await graphClient.Reports.GetOffice365ActivationsUserCounts()
    .Request()
    .GetAsync();

```