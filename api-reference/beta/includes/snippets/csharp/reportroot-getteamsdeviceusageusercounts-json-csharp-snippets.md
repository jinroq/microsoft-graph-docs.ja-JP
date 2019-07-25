---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 2c323db233abb418d2ef9a0a20ec7eeb5c1b16bd
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35871824"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getTeamsDeviceUsageUserCounts = await graphClient.Reports
    .GetTeamsDeviceUsageUserCounts('D7')
    .Request()
    .GetAsync();

```