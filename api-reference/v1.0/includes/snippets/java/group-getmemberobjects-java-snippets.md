---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: e1f3af531d6fa4caf8d39120fae950b8912c3b49
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35889282"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

boolean securityEnabledOnly = False;

graphClient.groups("{id}")
    .getMemberObjects(securityEnabledOnly)
    .buildRequest()
    .post();

```