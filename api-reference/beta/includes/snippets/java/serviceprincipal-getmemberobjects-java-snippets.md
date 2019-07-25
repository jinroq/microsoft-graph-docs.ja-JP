---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: c87976a67b143bbccee964f52c526bc6146346a2
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35870125"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

boolean securityEnabledOnly = True;

graphClient.servicePrincipals("{id}")
    .getMemberObjects(securityEnabledOnly)
    .buildRequest()
    .post();

```