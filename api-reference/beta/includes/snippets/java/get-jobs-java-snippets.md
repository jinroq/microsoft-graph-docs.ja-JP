---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 7b5928f6e6885265444980491d67c8a7d531fa62
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35869362"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISynchronizationJobCollectionPage jobs = graphClient.servicePrincipals("{id}").synchronization().jobs()
    .buildRequest()
    .get();

```