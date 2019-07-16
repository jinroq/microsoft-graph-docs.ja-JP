---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: ab8bde42fb4ca337230599efbf7c4da029724608
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35740013"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Devices["{id}"]
    .Request()
    .DeleteAsync();

```