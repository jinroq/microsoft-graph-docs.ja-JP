---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 9339918ea5335ba43acad5af7121c15603be954d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35485807"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getOffice365ActiveUserCounts = await graphClient.Reports.GetOffice365ActiveUserCounts('D7')
    .Request()
    .GetAsync();

```