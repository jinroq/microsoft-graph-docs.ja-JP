---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 5440ed31d45771f32dadcd29054baeeacf3ad359
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35717597"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var site = await graphClient.Sites["{site-id}"]
    .Request()
    .GetAsync();

```