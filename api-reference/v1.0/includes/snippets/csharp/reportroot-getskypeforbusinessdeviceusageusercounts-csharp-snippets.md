---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 93441e0c5c37b3fe62283285d6d497cc06267bd2
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36349293"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetSkypeForBusinessDeviceUsageUserCounts("D7")
    .Request()
    .GetAsync();

```