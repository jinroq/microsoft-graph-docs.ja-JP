---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: c18a3e617e89748b6c11d1b8de81e664d6a8077e
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35713670"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var events = await graphClient.Groups["{id}"].Events
    .Request()
    .GetAsync();

```