---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: e3f405aed0f743680ef5eb1d3660c638c5b14b79
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35892313"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetSkypeForBusinessParticipantActivityMinuteCounts('D7')
    .Request()
    .GetAsync();

```