---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d23dc968d33e2279a2ec6f270756ca6a96738296
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35526862"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directorySetting = await graphClient.Settings["{id}"]
    .Request()
    .GetAsync();

```