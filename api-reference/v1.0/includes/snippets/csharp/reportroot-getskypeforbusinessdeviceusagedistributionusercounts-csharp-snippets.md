---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 2ed2217c8bd81bd7fff8429f732c89f0016b4dab
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35471614"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetSkypeForBusinessDeviceUsageDistributionUserCounts('D7')
    .Request()
    .GetAsync();

```