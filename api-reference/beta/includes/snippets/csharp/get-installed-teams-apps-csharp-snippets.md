---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 17a68e67ac476b5bf226dbf85dc640148de8f1fd
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35868320"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var installedApps = await graphClient.Teams["{id}"].InstalledApps
    .Request()
    .GetAsync();

```