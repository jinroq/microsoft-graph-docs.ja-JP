---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 4f99253ee6180efd29195f2e8c0bb45792274d6b
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35873422"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getOffice365GroupsActivityCounts = await graphClient.Reports
    .GetOffice365GroupsActivityCounts('D7')
    .Request()
    .GetAsync();

```