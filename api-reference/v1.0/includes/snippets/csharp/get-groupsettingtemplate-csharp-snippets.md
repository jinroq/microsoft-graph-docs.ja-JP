---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 59f4a53626df8990c049714a2864ead1a39ad91b
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35741174"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groupSettingTemplate = await graphClient.GroupSettingTemplates["{id}"]
    .Request()
    .GetAsync();

```