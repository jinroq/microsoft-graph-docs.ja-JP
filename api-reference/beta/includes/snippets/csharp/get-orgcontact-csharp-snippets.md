---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 05db449e89d98c30d065c682c2fc041fb00c5886
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35729105"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var orgContact = await graphClient.Contacts["{id}"]
    .Request()
    .GetAsync();

```