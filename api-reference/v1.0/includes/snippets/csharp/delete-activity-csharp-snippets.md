---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 74feb3e07eefdfa63b14f7cd644863b352828ca3
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35739578"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Activities["{activity-id}"]
    .Request()
    .DeleteAsync();

```