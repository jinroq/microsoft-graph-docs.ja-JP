---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 0e3c733fa85632c4fa77f179348ce64021b19c3a
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35893769"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetOneDriveActivityUserCounts('D7')
    .Request()
    .GetAsync();

```