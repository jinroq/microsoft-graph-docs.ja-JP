---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 881ec7bac57269dbf90029c04bc7ea76988cf56c
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35709009"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.App.Calls["{id}"]
    .Request()
    .DeleteAsync();

```