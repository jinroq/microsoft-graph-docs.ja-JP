---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: ca5b571dad3993a594da8b1197e4437174a38d76
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35732402"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var messages = await graphClient.Me.Messages
    .Request()
    .Select( e => new {
             e.Sender,
             e.Subject 
             })
    .GetAsync();

```