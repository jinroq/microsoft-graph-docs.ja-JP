---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 3ad19815e67b7c750a07bd7c9af22133657994e4
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34477244"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attachment = await graphClient.Me.Messages["AAMkAGUzY5QKgAAA="].Attachments["AAMkAGUzY5QKgAAABEgAQAISJOe1FEqdNsMEQmpZjRW8="]
    .Request()
    .GetAsync();

```