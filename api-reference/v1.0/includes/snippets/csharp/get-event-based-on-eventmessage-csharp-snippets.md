---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 8732a356ca1dc70696960d8a4eab099eb6cc1385
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35735077"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = await graphClient.Me.Messages["AAMkADYAAAImV_jAAA="]
    .Request()
    .Expand("eventMessage/event")
    .GetAsync();

```