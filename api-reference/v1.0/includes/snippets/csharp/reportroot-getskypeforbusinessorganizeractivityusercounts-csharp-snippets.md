---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 3a373fcd7c577b47b3a8752cfd1d85d245db6e04
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35892336"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetSkypeForBusinessOrganizerActivityUserCounts('D7')
    .Request()
    .GetAsync();

```