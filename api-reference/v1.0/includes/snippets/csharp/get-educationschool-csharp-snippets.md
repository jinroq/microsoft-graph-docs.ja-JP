---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: b226f87522412109ff3163236b5a0554adb40105
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35735617"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationSchool = await graphClient.Education.Schools["{school-id}"]
    .Request()
    .GetAsync();

```