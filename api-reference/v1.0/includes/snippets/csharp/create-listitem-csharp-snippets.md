---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 2ce475a3f7582b880cbb32f87f01ae1cd5be5eea
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35731627"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var listItem = new ListItem
{
    Fields = new FieldValueSet
    {
        Title = "Widget",
        Color = "Purple",
        Weight = 32
    }
};

await graphClient.Sites["{site-id}"].Lists["{list-id}"].Items
    .Request()
    .AddAsync(listItem);

```