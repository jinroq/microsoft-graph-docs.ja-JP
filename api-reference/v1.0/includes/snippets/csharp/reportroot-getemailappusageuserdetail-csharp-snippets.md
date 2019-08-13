---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: c2c298c3e5e305d6852cc26865db64575ea53825
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36327320"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetEmailAppUsageUserDetail("D7")
    .Request()
    .GetAsync();

```