---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 9cc5b96a99d86271b47a7cccc8b771d03cf2b1ca
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34438428"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Classes["11022"]
    .Request()
    .DeleteAsync();

```