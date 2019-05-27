---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: b617e5f2335751e9c90345202daff4d20a93d67a
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34481423"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var serviceConfigurationRecords = await graphClient.Domains["{domain-name}"].ServiceConfigurationRecords
    .Request()
    .GetAsync();

```