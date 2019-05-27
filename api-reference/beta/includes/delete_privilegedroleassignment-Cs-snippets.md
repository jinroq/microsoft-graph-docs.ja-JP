---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 9f1138c81ea35469c4b3adbe170109f3688a0815
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34437651"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.PrivilegedRoleAssignments["{id}"]
    .Request()
    .DeleteAsync();

```