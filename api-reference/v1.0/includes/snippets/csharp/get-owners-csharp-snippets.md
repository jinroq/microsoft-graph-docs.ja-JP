---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 59c1e517b4fa3a55aa19392b193d6d9640311976
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35513841"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var installedApps = await graphClient.Teams["{id}"].InstalledApps
    .Request()
    .Expand("teamsAppDefinition")
    .GetAsync();

```