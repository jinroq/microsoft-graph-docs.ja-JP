---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 4a02b66cb311bbc274e643b5cee2c1e43b3ba883
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35504656"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.SynchronizationProfiles["{id}"]
    .Reset()
    .Request()
    .PostAsync();

```