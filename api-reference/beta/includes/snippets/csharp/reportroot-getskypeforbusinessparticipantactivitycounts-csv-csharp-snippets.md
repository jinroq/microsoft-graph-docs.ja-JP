---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 31da8ccfa96c371faa677bdb4ab19a73280dc61d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35504450"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getSkypeForBusinessParticipantActivityCounts = await graphClient.Reports.GetSkypeForBusinessParticipantActivityCounts('D7')
    .Request()
    .GetAsync();

```