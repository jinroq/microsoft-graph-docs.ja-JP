---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6846155f248d746ad775cccb0214f6fa3e19c480
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35858467"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IGroupLifecyclePolicyCollectionPage groupLifecyclePolicies = graphClient.groups("{id}").groupLifecyclePolicies()
    .buildRequest()
    .get();

```