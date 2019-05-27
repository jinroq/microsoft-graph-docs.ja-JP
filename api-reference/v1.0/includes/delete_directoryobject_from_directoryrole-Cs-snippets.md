---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a3b5c0c800d2ffc520322ca50da091f8ebffaa13
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34459308"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.DirectoryRoles["{id}"].Members["{id}"]
    .Request()
    .DeleteAsync();

```