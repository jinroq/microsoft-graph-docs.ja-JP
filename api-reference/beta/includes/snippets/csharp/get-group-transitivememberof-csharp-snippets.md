---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: ec497cedfc8d21e493c1fe275f1a1d5ceaa9eaf4
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35711949"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var transitiveMemberOf = await graphClient.Groups["{id}"].TransitiveMemberOf
    .Request()
    .GetAsync();

```