---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 45c6b8e2110701b835958ee57431ad855fca0eb8
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35871535"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getYammerDeviceUsageUserCounts = await graphClient.Reports
    .GetYammerDeviceUsageUserCounts('D7')
    .Request()
    .GetAsync();

```