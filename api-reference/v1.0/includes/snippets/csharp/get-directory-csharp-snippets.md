---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 95061fa350a4a7497da2f1277b3642ace5cfaaf7
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35513485"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = await graphClient.Directory.DeletedItems["{object-id}"]
    .Request()
    .GetAsync();

```