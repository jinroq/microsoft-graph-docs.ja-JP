---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: b255c4ac0e5b284db533844f82a26dc50b07d701
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35873081"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getOneDriveActivityUserDetail = await graphClient.Reports
    .GetOneDriveActivityUserDetail('D7')
    .Request()
    .GetAsync();

```