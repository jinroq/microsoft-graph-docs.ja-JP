---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a03effb282187ca1cfc84a893fe53773784299e5
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36371627"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetOneDriveUsageAccountDetail("D7")
    .Request()
    .GetAsync();

```