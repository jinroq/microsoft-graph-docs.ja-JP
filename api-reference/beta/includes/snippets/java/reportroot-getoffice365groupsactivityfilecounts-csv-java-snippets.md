---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 78b91b09691fa66359eb186075e8d27f7f86abf1
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36360390"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IOffice365GroupsActivityFileCountsCollectionPage getOffice365GroupsActivityFileCounts = graphClient.reports()
    .getOffice365GroupsActivityFileCounts("D7")
    .buildRequest()
    .get();

```