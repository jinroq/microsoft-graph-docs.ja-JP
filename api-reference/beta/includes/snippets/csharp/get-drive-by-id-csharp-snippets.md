---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 64e3eda9e9f75d4ccd2f5770d828837f2493076a
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35504178"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var drive = await graphClient.Drives["{driveId}"]
    .Request()
    .GetAsync();

```