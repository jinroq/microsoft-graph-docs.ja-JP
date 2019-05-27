---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: dd6f968606f74e19e4ad6708b11231f8c4052244
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34437567"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.ProgramControls["7e59d237-2fb0-4e5d-b7bb-d4f9f9129213"]
    .Request()
    .DeleteAsync();

```