---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: b28631a00c285f8556e5cbe6a913672ed2cd600b
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35741223"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groupSetting = new GroupSetting
{
    DisplayName = "displayName-value",
    TemplateId = "templateId-value",
    Values = new List<SettingValue>()
    {
        new SettingValue
        {
            Name = "name-value",
            Value = "value-value"
        }
    }
};

await graphClient.GroupSettings
    .Request()
    .AddAsync(groupSetting);

```