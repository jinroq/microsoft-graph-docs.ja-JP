---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 1b759c885c62ce6e9aff7f9c7377464cdee329f3
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35872118"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getSkypeForBusinessParticipantActivityCounts = await graphClient.Reports
    .GetSkypeForBusinessParticipantActivityCounts('D7')
    .Request()
    .GetAsync();

```