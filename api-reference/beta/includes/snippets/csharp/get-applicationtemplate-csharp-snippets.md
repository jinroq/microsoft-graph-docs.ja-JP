---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 886da2bf000935b475cbfba040164a3fe3d28ef3
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35486890"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var applicationTemplate = await graphClient.ApplicationTemplates["{id}"]
    .Request()
    .GetAsync();

```