---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 4b2c7b60c1b1e6fbb91d4af0e4cd81ae9dcad03c
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35881182"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Me.CalendarView
    .Delta()
    .Request()
    .Header("Prefer","odata.maxpagesize=2")
    .GetAsync();

```