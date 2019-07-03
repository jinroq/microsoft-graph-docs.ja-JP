---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 59bf2b57c658d0633094613383d7524d43c8085f
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35504321"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me
    .InvalidateAllRefreshTokens()
    .Request()
    .PostAsync();

```