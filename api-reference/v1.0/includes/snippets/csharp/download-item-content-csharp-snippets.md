---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 633928dc0357c5f3715993b373140ae2280d498d
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35739039"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var items = await graphClient.Me.Drive.Items["{item-id}"]
    .Request()
    .Select( e => new {
             e.Content 
             })
    .GetAsync();

var content = items.Content;

```