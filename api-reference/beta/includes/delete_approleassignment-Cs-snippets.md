---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 2be210960b5584ff9fa182850d5d03e63f2dab89
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34439030"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.AppRoleAssignments["{id}"]
    .Request()
    .DeleteAsync();

```