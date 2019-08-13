---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 0cc3859554222c40404b205cd0cef38513b43f19
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36320606"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetSkypeForBusinessPeerToPeerActivityMinuteCounts("D7")
    .Request()
    .GetAsync();

```