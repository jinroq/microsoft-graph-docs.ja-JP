---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 753924d1306e40f73b4c3db02ea1a848ca6b6c02
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35873122"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getOneDriveActivityUserCounts = await graphClient.Reports
    .GetOneDriveActivityUserCounts('D7')
    .Request()
    .GetAsync();

```