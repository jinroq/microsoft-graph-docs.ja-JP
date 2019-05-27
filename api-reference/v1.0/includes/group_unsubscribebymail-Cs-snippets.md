---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 7f05a61da2e621dd6518bb7032f4e146719d5d71
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34482368"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Groups["{id}"]
    .UnsubscribeByMail()
    .Request()
    .PostAsync();

```