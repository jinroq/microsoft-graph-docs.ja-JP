---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d0b07faa09a4ad952dac15b03023b4ac4feff510
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34473933"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var assignments = await graphClient.PrivilegedRoles["{id}"].Assignments
    .Request()
    .GetAsync();

```