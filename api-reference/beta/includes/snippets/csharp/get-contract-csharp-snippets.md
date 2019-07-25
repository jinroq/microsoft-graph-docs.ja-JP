---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 7f564744aef5a15791cc14d91d3c7e596afa3f17
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35707334"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contracts = await graphClient.Contracts
    .Request()
    .GetAsync();

```