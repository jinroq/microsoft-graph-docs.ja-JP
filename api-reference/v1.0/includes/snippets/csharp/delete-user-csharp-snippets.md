---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 02727a1c2499e558f1d2b6584ccf7a2c4f55a9b7
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35715021"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Users["{user-id}"]
    .Request()
    .DeleteAsync();

```