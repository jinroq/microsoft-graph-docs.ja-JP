---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 19b99fe6533903f442f47dd11f11909dad2aad96
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34437707"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Planner.Buckets["'id'"]
    .Request()
    .Header("If-Match","W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc=\"")
    .DeleteAsync();

```