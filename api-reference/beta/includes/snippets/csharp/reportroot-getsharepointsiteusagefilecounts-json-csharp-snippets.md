---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 5e995c4164949a18399212795152c664b2855a6d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35872660"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getSharePointSiteUsageFileCounts = await graphClient.Reports
    .GetSharePointSiteUsageFileCounts('D7')
    .Request()
    .GetAsync();

```