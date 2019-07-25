---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 1c99fbc336310bf44f23fcfabdf4f187946727bf
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35895544"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var memberOf = await graphClient.Contacts["{id}"].MemberOf
    .Request()
    .GetAsync();

```