---
description: 自動生成されたファイル。 変更しないでください
ms.openlocfilehash: c8ce6fd9df6ba0a7d47294dc9e9d699c81576de6
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35880767"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var calendars = await graphClient.Me.Calendars
    .Request()
    .GetAsync();

```