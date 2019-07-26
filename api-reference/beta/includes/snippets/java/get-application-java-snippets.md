---
description: 自動生成されたファイル。 変更しないでください
ms.openlocfilehash: 511df171efbcf38cd542e8d7a27a29c2fc5c66a2
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35855286"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Application application = graphClient.applications("{id}")
    .buildRequest()
    .get();

```