---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 672ec71879101810db62196e93b61fa83f4e1d77
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35721208"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var notebook = await graphClient.Me.Onenote.Notebooks["{id}"]
    .Request()
    .GetAsync();

```