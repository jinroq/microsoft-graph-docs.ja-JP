---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: c8ce6fd9df6ba0a7d47294dc9e9d699c81576de6
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34457060"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var calendars = await graphClient.Me.Calendars
    .Request()
    .GetAsync();

```