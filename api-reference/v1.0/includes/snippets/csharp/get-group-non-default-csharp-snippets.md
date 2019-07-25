---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 5dae900427d3e2b59152efc8d6b5cc3efe4cca5e
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35732508"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var group = await graphClient.Groups["b320ee12-b1cd-4cca-b648-a437be61c5cd"]
    .Request()
    .Select( e => new {
             e.AllowExternalSenders,
             e.AutoSubscribeNewMembers,
             e.IsSubscribedByMail,
             e.UnseenCount 
             })
    .GetAsync();

```