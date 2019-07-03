---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: e6aa7ae895baade00992d77d1abe0efb7721deb4
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35526629"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var privilegedRoleSummary = await graphClient.PrivilegedRoles["{id}"].Summary
    .Request()
    .GetAsync();

```