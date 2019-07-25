---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 9885e75daaea73979ca4ed6728d17d81052f3c72
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35883939"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var childFolders = await graphClient.Me.ContactFolders["{id}"].ChildFolders
    .Request()
    .GetAsync();

```