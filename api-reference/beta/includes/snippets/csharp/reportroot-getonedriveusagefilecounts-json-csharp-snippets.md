---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: efcc5891d38122349b5e233428bb6a614011b260
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35526050"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getOneDriveUsageFileCounts = await graphClient.Reports.GetOneDriveUsageFileCounts('D7')
    .Request()
    .GetAsync();

```