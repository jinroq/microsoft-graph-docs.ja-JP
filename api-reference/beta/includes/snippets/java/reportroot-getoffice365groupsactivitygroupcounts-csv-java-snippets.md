---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 453022f17641c2b7b6949e135fc5b5e5adee8556
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35873311"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IOffice365GroupsActivityGroupCountsCollectionPage getOffice365GroupsActivityGroupCounts = graphClient.reports()
    .getOffice365GroupsActivityGroupCounts('D7')
    .buildRequest()
    .get();

```