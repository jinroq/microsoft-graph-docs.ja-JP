---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 70b3b15952cc2191bee96ec8066706e2ca546e88
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35873424"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IOffice365GroupsActivityCountsCollectionPage getOffice365GroupsActivityCounts = graphClient.reports()
    .getOffice365GroupsActivityCounts('D7')
    .buildRequest()
    .get();

```