---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 5a74e81846887fa618af9055f20098e41750ebeb
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35870179"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.ServicePrincipals
    .Delta()
    .Request()
    .GetAsync();

```