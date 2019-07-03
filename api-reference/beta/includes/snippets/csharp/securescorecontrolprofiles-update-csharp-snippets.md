---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 48c3f32873a31ca3d3ee7b1a9a9275fd9a7ae2c6
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35486094"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var secureScoreControlProfile = new SecureScoreControlProfile
{
    ControlStateUpdates = "controlStateUpdates-value"
};

await graphClient.Security.SecureScoreControlProfiles["AdminMFA"]
    .Request()
    .UpdateAsync(secureScoreControlProfile);

```