---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 84418c60369e382d63841b4affdc0b4d6aacfc7c
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35856519"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Groups["{id}"].AcceptedSenders.References
    .Request()
    .DeleteAsync();

```