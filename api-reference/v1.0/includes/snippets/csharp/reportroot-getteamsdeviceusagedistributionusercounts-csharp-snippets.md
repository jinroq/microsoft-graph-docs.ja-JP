---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 0f1d362d70a8b652ae95250ecec26df8e13e3a0b
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35738115"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetTeamsDeviceUsageDistributionUserCounts('D7')
    .Request()
    .GetAsync();

```