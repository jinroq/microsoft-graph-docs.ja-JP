---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 01d6c26977f056a8c8d6cff431ff39463a67eb77
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35706024"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var children = await graphClient.Drives["{drive-id}"].Items["{item-id}"].Children
    .Request()
    .GetAsync();

```