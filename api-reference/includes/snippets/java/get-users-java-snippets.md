---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6170c5040dc0c64eb61a57dc16bc4af939b3c716
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35897125"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

User user = graphClient.users("{user-id}")
    .buildRequest()
    .get();

```