---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 4d27212649d395513c839454a9d624d861906b19
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35533611"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Me.CalendarView.Delta()
    .Request()
    .Header("Prefer","odata.maxpagesize=2")
    .SkipToken("R0usmcCM996atia_s")
    .GetAsync();

```