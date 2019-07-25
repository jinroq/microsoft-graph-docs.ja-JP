---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 98e625b910e4df40952a545b05b9b5e4ce24bb61
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35706347"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directorySettingTemplates = await graphClient.DirectorySettingTemplates
    .Request()
    .GetAsync();

```