---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: db4c13d8b3bd2fd94e34ce6dc45c486733b9167e
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34447720"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerBucketTaskBoardTaskFormat = await graphClient.Planner.Tasks["01gzSlKkIUSUl6DF_EilrmQAKDhh"].BucketTaskBoardFormat
    .Request()
    .GetAsync();

```