---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: fc3e4d190cc84edc7be903228c5d9d8bb10cfb10
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35514559"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var driveItem = await graphClient.Me.Drive.Root
    .Request()
    .GetAsync();

```