---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 0a963a9d109ec1a15bfb2061967fd76a0df6b0a3
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34467505"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contacts = await graphClient.Me.Contacts
    .Request()
    .GetAsync();

```