---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 18aed4242cdbdd63233d06a89e256c7dd5cfb6e3
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/19/2019
ms.locfileid: "36460988"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationRubric = new EducationRubric
{
    DisplayName = "Example Credit Rubric after display name patch"
};

await graphClient.Education.Me.Rubrics["{id}"]
    .Request()
    .UpdateAsync(educationRubric);

```