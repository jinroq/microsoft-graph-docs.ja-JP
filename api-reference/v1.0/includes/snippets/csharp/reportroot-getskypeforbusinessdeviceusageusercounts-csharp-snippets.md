---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a07cedc36f6dae5a6d5082c7df1304c39c802710
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35892455"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetSkypeForBusinessDeviceUsageUserCounts('D7')
    .Request()
    .GetAsync();

```