---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 576455c14e1235b36842631d076f0d76aac5eefd
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34479617"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationClass = await graphClient.Education.Classes["{class-id}"]
    .Request()
    .GetAsync();

```