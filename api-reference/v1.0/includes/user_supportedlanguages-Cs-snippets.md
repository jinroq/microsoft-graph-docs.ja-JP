---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 9b71fd0bdd2c1692f35c80901c23216cf324f021
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34454483"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var supportedLanguages = await graphClient.Me.Outlook.SupportedLanguages()
    .Request()
    .GetAsync();

```