---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d973a7c3c7fa1a79f8f00ab048ccff54a78561a1
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35886828"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

GroupLifecyclePolicy groupLifecyclePolicy = new GroupLifecyclePolicy();
groupLifecyclePolicy.groupLifetimeInDays = 100;
groupLifecyclePolicy.managedGroupTypes = "Selected";
groupLifecyclePolicy.alternateNotificationEmails = "admin@contoso.com";

graphClient.groupLifecyclePolicies()
    .buildRequest()
    .post(groupLifecyclePolicy);

```