---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 0a4dd2963e90c4c3b9983aab9d786fa9276c2afa
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35707538"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contact = await graphClient.Me.Contacts["AAMkAGI2THk0AAA="]
    .Request()
    .GetAsync();

```