---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 43a998cfdba08d5e306ad6f8179847c7dd1dc562
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35871626"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getTeamsUserActivityUserDetail = await graphClient.Reports
    .GetTeamsUserActivityUserDetail('D7')
    .Request()
    .GetAsync();

```