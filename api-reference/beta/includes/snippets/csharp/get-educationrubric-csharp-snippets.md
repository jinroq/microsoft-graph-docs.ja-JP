---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: b026fd4533468825885e3bc06854cbf179c77b67
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/19/2019
ms.locfileid: "36461032"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationRubric = await graphClient.Education.Me.Rubrics["{id}"]
    .Request()
    .GetAsync();

```