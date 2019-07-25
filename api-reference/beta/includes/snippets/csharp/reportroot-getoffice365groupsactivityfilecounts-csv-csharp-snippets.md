---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 03feab4f435aa8e97b01dd3a085b17e6d3131cfa
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35873381"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getOffice365GroupsActivityFileCounts = await graphClient.Reports
    .GetOffice365GroupsActivityFileCounts('D7')
    .Request()
    .GetAsync();

```