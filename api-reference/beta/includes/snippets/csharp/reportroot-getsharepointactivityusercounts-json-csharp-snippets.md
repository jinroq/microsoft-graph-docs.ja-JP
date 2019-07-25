---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6af0cad8405a58bf3957850bd28d0a99526a836f
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35872822"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getSharePointActivityUserCounts = await graphClient.Reports
    .GetSharePointActivityUserCounts('D7')
    .Request()
    .GetAsync();

```