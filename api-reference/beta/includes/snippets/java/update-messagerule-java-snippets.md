---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: e3243badf01545c5cde8e0abec7f6d16e0d75f80
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35879302"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MessageRule messageRule = new MessageRule();
messageRule.displayName = "Important from partner";
MessageRuleActions actions = new MessageRuleActions();
actions.markImportance = Importance.HIGH;
messageRule.actions = actions;

graphClient.me().mailFolders("inbox").messageRules("AQAAAJ5dZqA=")
    .buildRequest()
    .patch(messageRule);

```