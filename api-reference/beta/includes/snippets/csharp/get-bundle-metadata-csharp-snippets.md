---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6d86de3dd36f93d93966bc6e4f4e9d550dfb8deb
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/30/2019
ms.locfileid: "35932846"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var driveItem = await graphClient.Drive.Bundles["{bundle-id}"]
    .Request()
    .GetAsync();

```