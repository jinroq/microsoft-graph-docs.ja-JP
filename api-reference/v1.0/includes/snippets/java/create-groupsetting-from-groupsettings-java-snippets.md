---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 2fafcce6e473d1f1d8227ac85f16d66048251b59
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35884119"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

GroupSetting groupSetting = new GroupSetting();
groupSetting.displayName = "displayName-value";
groupSetting.templateId = "templateId-value";
LinkedList<SettingValue> valuesList = new LinkedList<SettingValue>();
SettingValue values = new SettingValue();
values.name = "name-value";
values.value = "value-value";
valuesList.add(values);
groupSetting.values = valuesList;

graphClient.groupSettings()
    .buildRequest()
    .post(groupSetting);

```