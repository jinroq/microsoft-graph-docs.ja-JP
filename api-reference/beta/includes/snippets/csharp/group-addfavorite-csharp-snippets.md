---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: f953d9ad67ca4558856cef72c7b961b5c9fe027d
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35713865"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Groups["{id}"]
    .AddFavorite()
    .Request()
    .PostAsync();

```