---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d591d12f30b4e37bc061090269c819abcb2d0e82
ms.sourcegitcommit: d8a58221ed1f2b7b7073fd621da4737e11ba53c5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/11/2019
ms.locfileid: "36838842"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var reason = RejectReason.Busy;

await graphClient.App.Calls["57dab8b1-894c-409a-b240-bd8beae78896"]
    .Reject(reason,callbackUri)
    .Request()
    .PostAsync();

```