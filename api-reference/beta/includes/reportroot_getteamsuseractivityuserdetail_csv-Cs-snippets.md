---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: c8d727f6db97640905cf5ec9ca2ef7da2614d90c
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34462874"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getTeamsUserActivityUserDetail = await graphClient.Reports.GetTeamsUserActivityUserDetail('D7')
    .Request()
    .GetAsync();

```