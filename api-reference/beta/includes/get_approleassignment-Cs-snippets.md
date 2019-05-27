---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: e8d5d291c4d97f513e04353f49e21b1d755a8f27
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34473982"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var appRoleAssignment = await graphClient.AppRoleAssignments["{id}"]
    .Request()
    .GetAsync();

```