---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: da3483616be48434ac83dc126a7bdda639dc5205
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35504416"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var servicePrincipal = await graphClient.ServicePrincipals["{id}"]
    .Request()
    .GetAsync();

```