---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: b5c9f1ce4bc5cfa83417079d29586f801cc24ac8
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35883273"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDomainCollectionPage domains = graphClient.domains()
    .buildRequest()
    .get();

```