---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d93fa7cb5282aa6e0ad2ae4b4fb9cf925828b375
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35717512"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sitePage = await graphClient.Sites["{site-id}"].Pages["{page-id}"]
    .Request()
    .GetAsync();

```