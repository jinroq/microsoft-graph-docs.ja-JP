---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 120fa00b13de5f92b79cc5a1624dba4f9f7d0469
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35890132"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

boolean securityEnabledOnly = True;

graphClient.directoryObjects("{object-id}")
    .getMemberObjects(securityEnabledOnly)
    .buildRequest()
    .post();

```