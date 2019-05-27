---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: efbee63257a4527add53e837ee10a1d8e575f354
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34471656"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationAssignmentResource = await graphClient.Education.Classes["11021"].Assignments["19002"].Resources["22002"]
    .Request()
    .GetAsync();

```