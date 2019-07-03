---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6d644451770f4a3507c225656445cd4c14f3d4bc
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35485241"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getYammerDeviceUsageUserDetail = await graphClient.Reports.GetYammerDeviceUsageUserDetail('D7')
    .Request()
    .GetAsync();

```