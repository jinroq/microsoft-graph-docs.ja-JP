---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 4885f2298ef8580056a553b8f5c049f361864712
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35873904"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getEmailAppUsageUserCounts = await graphClient.Reports
    .GetEmailAppUsageUserCounts('D7')
    .Request()
    .GetAsync();

```