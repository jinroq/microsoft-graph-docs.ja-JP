---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 1a3c6575e38c5a3c44b4b0206669325ff90ffc9d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35871611"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getYammerDeviceUsageUserDetail = await graphClient.Reports
    .GetYammerDeviceUsageUserDetail('D7')
    .Request()
    .GetAsync();

```