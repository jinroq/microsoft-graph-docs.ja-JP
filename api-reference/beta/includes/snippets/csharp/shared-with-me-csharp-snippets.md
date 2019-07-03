---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 8e845e305eb7f10adb4b737b04bd5c6660f0dc84
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35526240"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sharedWithMe = await graphClient.Me.Drive.SharedWithMe()
    .Request()
    .GetAsync();

```