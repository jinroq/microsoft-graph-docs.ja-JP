---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 1c038417fcc79621c6a19fdd10cb65b761a45dc8
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35526245"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.ServicePrincipals.Delta()
    .Request()
    .GetAsync();

```