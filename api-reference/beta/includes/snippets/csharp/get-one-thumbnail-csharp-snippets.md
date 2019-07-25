---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 8a2135be2fa313fd8cee336096932609a25f7c53
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35706167"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var {size} = await graphClient.Me.Drive.Items["{item-id}"].Thumbnails["{thumb-id}"].{size}
    .Request()
    .GetAsync();

```