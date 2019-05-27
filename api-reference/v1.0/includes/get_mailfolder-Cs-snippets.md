---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 0b8faa3f6067d106d381d4216380792b02041121
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34477874"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var mailFolder = await graphClient.Me.MailFolders["{id}"]
    .Request()
    .GetAsync();

```