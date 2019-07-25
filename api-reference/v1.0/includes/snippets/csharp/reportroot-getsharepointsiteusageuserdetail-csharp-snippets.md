---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: b2130287015c57569702c7caf77d74fa7613e3d4
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35893496"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetSharePointSiteUsageDetail('D7')
    .Request()
    .GetAsync();

```