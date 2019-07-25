---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 0987540388dd16c6023038084184ca527a806639
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35888198"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Message message = new Message();
message.isRead = "true";

graphClient.me().messages("{id}")
    .buildRequest()
    .patch(message);

```