---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: be5a5c523727e3ad0b162f4aba5f1c2647ee8486
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34444343"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var applications = await graphClient.Applications
    .Request()
    .GetAsync();

```