---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 4bf9214aaf694fc1ebfb4a87423825ea72cab649
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35733517"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var domain = await graphClient.Domains["contoso.com"]
    .Request()
    .GetAsync();

```