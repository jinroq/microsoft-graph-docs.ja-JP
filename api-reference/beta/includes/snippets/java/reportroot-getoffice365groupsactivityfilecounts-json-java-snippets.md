---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: f7be205802e5d8cf2bf8859c66c5ed0fbf5bb892
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35873379"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IOffice365GroupsActivityFileCountsCollectionPage getOffice365GroupsActivityFileCounts = graphClient.reports()
    .getOffice365GroupsActivityFileCounts('D7')
    .buildRequest()
    .get();

```