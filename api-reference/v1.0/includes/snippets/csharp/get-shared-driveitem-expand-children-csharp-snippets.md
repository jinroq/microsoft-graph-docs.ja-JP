---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 983a9f6179590eba3a833fadd6cbdcc3a47b00c9
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35736871"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var driveItem = await graphClient.Shares["{shareIdOrUrl}"].DriveItem
    .Request()
    .Expand("children")
    .GetAsync();

```