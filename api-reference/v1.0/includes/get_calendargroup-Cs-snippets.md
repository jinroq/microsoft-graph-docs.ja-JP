---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 79f310d7fd77e2896bb03a855b221e835952b27d
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34475235"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var calendarGroup = await graphClient.Me.CalendarGroups["{id}"]
    .Request()
    .GetAsync();

```