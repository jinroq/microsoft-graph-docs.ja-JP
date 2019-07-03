---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 10870e1fb6a59ea59be19321d11dc1bc5056d4ee
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35496336"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var group = await graphClient.Groups["b320ee12-b1cd-4cca-b648-a437be61c5cd"]
    .Request()
    .GetAsync();

```