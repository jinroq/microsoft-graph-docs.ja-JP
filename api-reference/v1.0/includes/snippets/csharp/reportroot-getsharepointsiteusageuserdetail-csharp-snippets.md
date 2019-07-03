---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 75f5af482936505e9a70aeb6cc5863e964e887bf
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35495597"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetSharePointSiteUsageDetail('D7')
    .Request()
    .GetAsync();

```