---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: e5abc9ccd9e4790bcaa7b5dda3fdadc3d114ac0a
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35707742"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var chats = await graphClient.Users["{id}"].Chats
    .Request()
    .GetAsync();

```