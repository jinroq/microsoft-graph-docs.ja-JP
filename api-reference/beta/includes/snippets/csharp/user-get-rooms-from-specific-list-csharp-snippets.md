---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6b770f480f2444cb1b60981be797b39bf82a8cf2
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36362463"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var findRooms = await graphClient.Me
    .FindRooms("Building2Rooms@contoso.onmicrosoft.com")
    .Request()
    .GetAsync();

```