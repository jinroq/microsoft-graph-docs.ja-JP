---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: fcb535e44664ba3fea67ce37dbc20ec012220faa
ms.sourcegitcommit: d8a58221ed1f2b7b7073fd621da4737e11ba53c5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/11/2019
ms.locfileid: "36846143"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = new Message
{
    IsRead = true
};

await graphClient.Me.Messages["{id}"]
    .Request()
    .UpdateAsync(message);

```