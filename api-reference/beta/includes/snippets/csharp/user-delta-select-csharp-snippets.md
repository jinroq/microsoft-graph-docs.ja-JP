---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 3c72fc0fec734d1b65578dfe25b13794355ba9c5
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35867837"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Users
    .Delta()
    .Request()
    .Select( e => new {
             e.DisplayName,
             e.JobTitle,
             e.MobilePhone 
             })
    .GetAsync();

```