---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: bb91a59a9e03b78194022d291c5d2fdea542bcb3
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34843543"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var drive = await graphClient.Drives["{drive-id}"]
    .Request()
    .GetAsync();

```