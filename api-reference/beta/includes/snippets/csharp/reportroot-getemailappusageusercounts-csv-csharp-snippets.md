---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 05e3192174d0688c090d0570f2f9fb76c7e37400
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35486457"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getEmailAppUsageUserCounts = await graphClient.Reports.GetEmailAppUsageUserCounts('D7')
    .Request()
    .GetAsync();

```