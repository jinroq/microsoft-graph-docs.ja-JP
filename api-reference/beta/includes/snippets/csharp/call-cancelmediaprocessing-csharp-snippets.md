---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: ea35d4442b48be4ef2502fcbecf5065a395032db
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35526261"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var all = true;

var clientContext = "clientContext-value";

await graphClient.App.Calls["{id}"]
    .CancelMediaProcessing(all,clientContext)
    .Request()
    .PostAsync();

```