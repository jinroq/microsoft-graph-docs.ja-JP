---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: c9289cec5e9d4b18a11dcad7fcaee45017eeef23
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35504442"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getSkypeForBusinessParticipantActivityUserCounts = await graphClient.Reports.GetSkypeForBusinessParticipantActivityUserCounts('D7')
    .Request()
    .GetAsync();

```