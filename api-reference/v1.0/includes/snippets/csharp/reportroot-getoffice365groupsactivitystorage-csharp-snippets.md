---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 2c885601a2957aa440d3744402849d0cdae36ff2
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35893819"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetOffice365GroupsActivityStorage('D7')
    .Request()
    .GetAsync();

```