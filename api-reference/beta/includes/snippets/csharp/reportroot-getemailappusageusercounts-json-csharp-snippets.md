---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 732cc46e63424b1a70e197767858cc8d0a4e629b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36308512"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getEmailAppUsageUserCounts = await graphClient.Reports
    .GetEmailAppUsageUserCounts("D7")
    .Request()
    .GetAsync();

```