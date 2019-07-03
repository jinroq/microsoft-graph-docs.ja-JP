---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 39548837e8e033276140337c3ff72d35febf2db7
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35503445"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Applications["{id}"]
    .Request()
    .DeleteAsync();

```