---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: f52bee2b1954d4823e901154be63d50e4f4205f6
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35862880"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ConversationThread conversationThread = new ConversationThread();
conversationThread.additionalDataManager().put("@odata.type", new JsonPrimitive("#Microsoft.OutlookServices.ConversationThread"));
conversationThread.isLocked = true;

graphClient.groups("{id}").threads("{id}")
    .buildRequest()
    .patch(conversationThread);

```