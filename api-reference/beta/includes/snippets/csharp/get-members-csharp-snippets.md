---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 900ffa40398aae5aee9592ff9d76bf2178aa98f2
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35705656"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var members = await graphClient.Education.Classes["11016"].Members
    .Request()
    .GetAsync();

```