---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6eb0effb655e8130e01889d06904b49f2a1f6c81
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35864640"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String clientContext = "d45324c1-fcb5-430a-902c-f20af696537c";

graphClient.app().calls("{id}")
    .subscribeToTone(clientContext)
    .buildRequest()
    .post();

```