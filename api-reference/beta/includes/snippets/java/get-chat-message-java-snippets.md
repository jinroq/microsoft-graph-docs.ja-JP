---
description: 自動生成されたファイル。 変更しないでください
ms.openlocfilehash: 5a326f6118e1e07e708550b17bd2bd9750e2b815
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35863580"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ChatMessage chatMessage = graphClient.me().chats("{id}").messages("{id}")
    .buildRequest()
    .get();

```