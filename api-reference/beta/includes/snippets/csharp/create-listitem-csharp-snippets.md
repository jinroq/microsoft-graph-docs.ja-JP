---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: fe232c0c5a555fde0f22c103ef110166fcb110d6
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35721803"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var fieldValueSet = new FieldValueSet
{
    Color = "Fuchsia",
    Quantity = 934
};

await graphClient.Sites["{site-id}"].Lists["{list-id}"].Items["{item-id}"].Fields
    .Request()
    .UpdateAsync(fieldValueSet);

```