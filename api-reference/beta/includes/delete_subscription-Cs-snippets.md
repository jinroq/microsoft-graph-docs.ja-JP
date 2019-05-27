---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 4794d8788d3d40150f96f03065ef5f486232c699
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34437483"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Subscriptions["{id}"]
    .Request()
    .DeleteAsync();

```