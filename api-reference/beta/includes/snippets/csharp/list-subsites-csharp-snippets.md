---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: dd5605e95268e9f85c8cc1ebc08fd259c2301fca
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35526284"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sites = await graphClient.Sites["{site-id}"].Sites
    .Request()
    .GetAsync();

```