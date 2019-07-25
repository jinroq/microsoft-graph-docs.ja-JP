---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 35544c71360fd0838daf2ef42625cc819177793f
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35863525"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ChatMessage chatMessage = new ChatMessage();
ItemBody body = new ItemBody();
body.content = "Hello world";
chatMessage.body = body;

graphClient.teams("{id}").channels("{id}").messages("{id}").replies()
    .buildRequest()
    .post(chatMessage);

```