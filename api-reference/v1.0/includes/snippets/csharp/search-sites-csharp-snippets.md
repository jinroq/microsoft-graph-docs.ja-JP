---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 83629738fcadcba26206e22aece568e4d8ddb8e9
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35471277"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("search", "{query}")
};

var sites = await graphClient.Sites
    .Request( queryOptions )
    .GetAsync();

```