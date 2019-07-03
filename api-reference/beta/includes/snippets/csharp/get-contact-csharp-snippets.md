---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 0a4dd2963e90c4c3b9983aab9d786fa9276c2afa
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35504688"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contact = await graphClient.Me.Contacts["AAMkAGI2THk0AAA="]
    .Request()
    .GetAsync();

```