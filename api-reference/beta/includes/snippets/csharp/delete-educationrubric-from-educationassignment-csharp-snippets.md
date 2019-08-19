---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: f3202c027fcde81b5744484b348414bd34ac41e6
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/19/2019
ms.locfileid: "36461204"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Me.Assignments["{id}"].Rubric.Reference
    .Request()
    .DeleteAsync();

```