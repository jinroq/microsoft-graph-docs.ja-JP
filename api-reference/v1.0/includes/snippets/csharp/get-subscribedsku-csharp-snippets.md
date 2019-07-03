---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 27243f32ce1690c651ae094c08e99b2c75415507
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35513925"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var subscribedSku = await graphClient.SubscribedSkus["{id}"]
    .Request()
    .GetAsync();

```