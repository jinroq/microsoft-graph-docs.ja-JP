---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 55367dc416bc635bc3f855d1c6df22c04bd2aee9
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36320497"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetTeamsDeviceUsageUserDetail("D7")
    .Request()
    .GetAsync();

```