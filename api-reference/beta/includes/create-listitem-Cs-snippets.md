---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: fe232c0c5a555fde0f22c103ef110166fcb110d6
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/29/2019
ms.locfileid: "34546843"
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