---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 9b2749d1388c873ed42ae0bb0e9e26bf392391e9
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36360691"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getEmailAppUsageVersionsUserCounts = await graphClient.Reports
    .GetEmailAppUsageVersionsUserCounts("D7")
    .Request()
    .GetAsync();

```