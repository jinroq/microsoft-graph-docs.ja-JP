---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 35d0af3bfa42f85c0b5ab350895a99f7b49d6ab9
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35721076"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = await graphClient.Contacts["{id}"].Manager
    .Request()
    .GetAsync();

```