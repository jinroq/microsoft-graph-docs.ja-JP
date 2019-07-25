---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 48c3f32873a31ca3d3ee7b1a9a9275fd9a7ae2c6
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35717940"
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