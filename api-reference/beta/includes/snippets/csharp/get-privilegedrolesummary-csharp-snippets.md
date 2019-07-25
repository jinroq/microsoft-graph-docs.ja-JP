---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: e6aa7ae895baade00992d77d1abe0efb7721deb4
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35728393"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var privilegedRoleSummary = await graphClient.PrivilegedRoles["{id}"].Summary
    .Request()
    .GetAsync();

```