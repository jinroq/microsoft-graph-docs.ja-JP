---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 320c7d198a7100a7fa39cc6db67802002fb77c39
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35861355"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String type = "view";

String password = "ThisIsMyPrivatePassword";

String scope = "anonymous";

graphClient.me().drive().items("{itemId}")
    .createLink(type,scope,expirationDateTime,password,message,recipientsList)
    .buildRequest()
    .post();

```