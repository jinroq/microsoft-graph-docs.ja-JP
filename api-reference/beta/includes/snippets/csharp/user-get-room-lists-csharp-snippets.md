---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6a6e93d95b4955725b680778bd8eb46626bc3dad
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35867756"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var findRoomLists = await graphClient.Me
    .FindRoomLists()
    .Request()
    .GetAsync();

```