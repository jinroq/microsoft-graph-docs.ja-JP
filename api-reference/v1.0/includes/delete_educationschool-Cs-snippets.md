---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: b6fa6bcf334d47b90b18e90969d049bf19672292
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34459187"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Schools["{school-id}"]
    .Request()
    .DeleteAsync();

```