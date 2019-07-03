---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 4230b4d478ad0b69657ac66f74adb2e00e0aa7ae
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35514333"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var comment = "comment-value";

var sendResponse = true;

await graphClient.Me.Events["{id}"]
    .TentativelyAccept(comment,sendResponse)
    .Request()
    .PostAsync();

```