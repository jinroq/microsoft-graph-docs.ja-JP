---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: f0ec5dd201a8c2694451935e9e68a8e4e87f4791
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35892495"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetSkypeForBusinessActivityUserDetail('D7')
    .Request()
    .GetAsync();

```