---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 0f0de65547b6beba04649ea5058fde1aef706934
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35895116"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var memberOf = await graphClient.Devices["{id}"].MemberOf
    .Request()
    .GetAsync();

```