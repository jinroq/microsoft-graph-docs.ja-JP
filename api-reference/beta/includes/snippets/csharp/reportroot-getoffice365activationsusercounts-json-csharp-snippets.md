---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 4a0f742098aa7d3c3fb81b73a8af84cb814119b4
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35873568"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getOffice365ActivationsUserCounts = await graphClient.Reports
    .GetOffice365ActivationsUserCounts()
    .Request()
    .GetAsync();

```