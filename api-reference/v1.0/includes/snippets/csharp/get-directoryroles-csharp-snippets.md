---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 80be132d0345accb780d2c9c1ddee8a6d9b9fb4e
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35733655"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryRoles = await graphClient.DirectoryRoles
    .Request()
    .GetAsync();

```