---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: e5bf8124be0fa5aede4e8a02f8fdf08061baf5e5
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36408446"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var agreement = new Agreement
{
    DisplayName = "displayName-value",
    IsViewingBeforeAcceptanceRequired = true
};

await graphClient.Agreements["{id}"]
    .Request()
    .UpdateAsync(agreement);

```