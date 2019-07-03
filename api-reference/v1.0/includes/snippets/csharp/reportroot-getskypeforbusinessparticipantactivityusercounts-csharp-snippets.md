---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: fbd2f275811581d162685518bb31da7129d1d015
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35463130"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetSkypeForBusinessParticipantActivityUserCounts('D7')
    .Request()
    .GetAsync();

```