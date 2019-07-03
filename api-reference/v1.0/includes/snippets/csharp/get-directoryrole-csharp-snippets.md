---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: dbdd24d583cf817b3cae81ec281714f8417322d2
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35472385"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryRole = await graphClient.DirectoryRoles["{id}"]
    .Request()
    .GetAsync();

```