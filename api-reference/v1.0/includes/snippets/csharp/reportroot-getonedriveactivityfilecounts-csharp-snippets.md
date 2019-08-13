---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 563d380b7164d54749dadb637bdd200e0278a061
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36373996"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetOneDriveActivityFileCounts("D7")
    .Request()
    .GetAsync();

```