---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 4bc643d9679acd60a8d47db55c766797a288d5d7
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35872891"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getSharePointActivityFileCounts = await graphClient.Reports
    .GetSharePointActivityFileCounts('D7')
    .Request()
    .GetAsync();

```