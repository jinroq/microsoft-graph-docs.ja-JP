---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 59c1e517b4fa3a55aa19392b193d6d9640311976
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35895132"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var installedApps = await graphClient.Teams["{id}"].InstalledApps
    .Request()
    .Expand("teamsAppDefinition")
    .GetAsync();

```