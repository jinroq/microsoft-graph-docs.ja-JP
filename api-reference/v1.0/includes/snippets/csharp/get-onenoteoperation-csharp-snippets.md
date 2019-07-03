---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: cbd840887e5837380483ad0e40797fb2e6331a3b
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35471453"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var onenoteOperation = await graphClient.Me.Onenote.Operations["{id}"]
    .Request()
    .GetAsync();

```