---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 32b90824ac622cc6ab682ac2166e8b4249efed91
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35862458"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = await graphClient.DirectoryObjects["delta"]
    .Request()
    .GetAsync();

```