---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: f879328da6bf2fda942721a62d571e879a794d2e
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35486648"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.ServicePrincipals["{id}"]
    .Request()
    .DeleteAsync();

```