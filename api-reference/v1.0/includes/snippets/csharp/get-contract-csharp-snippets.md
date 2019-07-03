---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 7f564744aef5a15791cc14d91d3c7e596afa3f17
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35513343"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contracts = await graphClient.Contracts
    .Request()
    .GetAsync();

```