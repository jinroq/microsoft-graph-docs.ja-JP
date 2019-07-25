---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d100e79f85ea48fe3f135f8996fb182df701a1ad
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35876787"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var rooms = await graphClient.Places["bldg2@contoso.com"].Microsoft.graph.roomlist.Rooms
    .Request()
    .GetAsync();

```