---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: c556f93aec55b10705ebb833655269afec652146
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35885901"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetYammerDeviceUsageUserCounts('D7')
    .Request()
    .GetAsync();

```