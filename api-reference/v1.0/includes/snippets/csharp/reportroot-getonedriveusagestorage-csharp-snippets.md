---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a220940bccce7c1abb4f81ad5c860cb348a3e1c8
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35893630"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetOneDriveUsageStorage('D7')
    .Request()
    .GetAsync();

```