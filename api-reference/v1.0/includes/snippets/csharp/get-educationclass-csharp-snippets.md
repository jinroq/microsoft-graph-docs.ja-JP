---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 576455c14e1235b36842631d076f0d76aac5eefd
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35715504"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationClass = await graphClient.Education.Classes["{class-id}"]
    .Request()
    .GetAsync();

```