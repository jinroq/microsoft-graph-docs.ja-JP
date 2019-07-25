---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: cffef970a55583a79202d9b31a5d0d75c8b535dd
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35715461"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var teachers = await graphClient.Education.Classes["{class-id}"].Teachers
    .Request()
    .GetAsync();

```