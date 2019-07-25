---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 92d5df78d677ad119f0cdec8d4b8afac677d532d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35871983"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getSkypeForBusinessParticipantActivityMinuteCounts = await graphClient.Reports
    .GetSkypeForBusinessParticipantActivityMinuteCounts('D7')
    .Request()
    .GetAsync();

```