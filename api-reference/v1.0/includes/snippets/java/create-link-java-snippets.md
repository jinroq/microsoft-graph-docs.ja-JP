---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 7272da8af392cc47851d86628f013abc2823a32e
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35881833"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String type = "view";

String scope = "anonymous";

graphClient.me().drive().items("{item-id}")
    .createLink(type,scope)
    .buildRequest()
    .post();

```