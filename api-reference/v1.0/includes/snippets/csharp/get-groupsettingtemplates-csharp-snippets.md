---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 44d00c7a706c3dabc1ea8b75126bc8f3cfc1d318
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35471244"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groupSettingTemplates = await graphClient.GroupSettingTemplates
    .Request()
    .GetAsync();

```