---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 59964e3c1c5efd356dad4e292bad15441688d782
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35872923"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getOneDriveUsageStorage = await graphClient.Reports
    .GetOneDriveUsageStorage('D7')
    .Request()
    .GetAsync();

```