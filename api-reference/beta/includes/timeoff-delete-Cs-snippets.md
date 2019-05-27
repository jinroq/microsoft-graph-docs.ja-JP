---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 3be0f4ffaa46cf424b5101cccb8667c7e9d0a02f
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34469280"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Teams["{teamId}"].Schedule.TimesOff["{timeOffId}"]
    .Request()
    .DeleteAsync();

```