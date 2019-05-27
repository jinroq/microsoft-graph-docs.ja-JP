---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 0c38dde77f759bcafa476f77e825ee6c00f7d566
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34448916"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = await graphClient.Me.Messages["AAMkAGI1AAAoZCfHAAA="]
    .Request()
    .GetAsync();

```