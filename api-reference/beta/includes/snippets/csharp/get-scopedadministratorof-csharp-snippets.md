---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: bac0f098e633c8839f11e356a4eb688e18c6192e
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35716484"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var scopedAdministratorOf = await graphClient.Me.ScopedAdministratorOf
    .Request()
    .GetAsync();

```