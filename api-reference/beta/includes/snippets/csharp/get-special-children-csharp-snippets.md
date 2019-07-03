---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 1541b331ef946860424fb6b943f88b2a23b818f2
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35504394"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var children = await graphClient.Me.Drive.Special["{name}"].Children
    .Request()
    .GetAsync();

```