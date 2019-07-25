---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 516eccfd5357af1e094100f056b3834acba0f596
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35873161"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getOneDriveActivityFileCounts = await graphClient.Reports
    .GetOneDriveActivityFileCounts('D7')
    .Request()
    .GetAsync();

```