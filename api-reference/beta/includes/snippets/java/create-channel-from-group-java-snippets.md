---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 28be228f8eaf3c972f5e8e2d6756502749fc32f4
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35864406"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Channel channel = new Channel();
channel.displayName = "Architecture Discussion";
channel.description = "This channel is where we debate all future architecture plans";

graphClient.teams("{id}").channels()
    .buildRequest()
    .post(channel);

```