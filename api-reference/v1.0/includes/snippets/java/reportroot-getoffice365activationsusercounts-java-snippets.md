---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 64db02f6c476ea9fa2e0d4f502d054627a8c5c3c
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35888535"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getOffice365ActivationsUserCounts()
    .buildRequest()
    .get();

```