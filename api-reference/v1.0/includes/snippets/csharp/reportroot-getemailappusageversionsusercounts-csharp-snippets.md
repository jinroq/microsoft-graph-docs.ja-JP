---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d175234894674f29e99eb9ca34d8fd42b51a7488
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35880399"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetEmailAppUsageVersionsUserCounts('D7')
    .Request()
    .GetAsync();

```