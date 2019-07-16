---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6c705ab4914cbf229f6a1e41d6a3fc0df3d52c48
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35741047"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contact = await graphClient.Me.Contacts["{id}"]
    .Request()
    .GetAsync();

```