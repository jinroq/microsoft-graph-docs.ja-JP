---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 4935196f6b87284aa2d01de589848a271e393c5f
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35893958"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetOffice365GroupsActivityDetail('D7')
    .Request()
    .GetAsync();

```