---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 8b9e744045935e56757e0470914f1b9deb0f3bdd
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/30/2019
ms.locfileid: "35931662"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Users["{id}"].Teamwork.InstalledApps["{id}"]
    .Request()
    .DeleteAsync();

```