---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 12d9a5707e6c6c23d76417f6f9dfc0e278a786b0
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35706522"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var drive = await graphClient.Users["{idOrUserPrincipalName}"].Drive
    .Request()
    .GetAsync();

```