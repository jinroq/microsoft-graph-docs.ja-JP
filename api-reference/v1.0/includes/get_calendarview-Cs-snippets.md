---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 16b59d90d94be2a6cdffb203bf1c8c537e0f787d
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34457011"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var calendarView = await graphClient.Me.CalendarView
    .Request()
    .GetAsync();

```