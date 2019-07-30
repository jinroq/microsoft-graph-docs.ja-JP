---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 9113c2337a936fdfec1d94116c6a451a39443f87
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/30/2019
ms.locfileid: "35933973"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var reason = RejectReason.None;

await graphClient.App.Calls["{id}"]
    .Reject(reason,callbackUri)
    .Request()
    .PostAsync();

```