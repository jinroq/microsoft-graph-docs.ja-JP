---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 4ea23e1a3c90e8e3a373d59ad6656926ad9444a3
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35893356"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetSharePointSiteUsageStorage('D7')
    .Request()
    .GetAsync();

```