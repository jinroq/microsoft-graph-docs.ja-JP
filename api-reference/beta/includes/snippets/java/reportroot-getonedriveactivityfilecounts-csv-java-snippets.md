---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: fee9dfd6ff6c058aedeba208abc18e440acbe8ef
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36360236"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISiteActivitySummaryCollectionPage getOneDriveActivityFileCounts = graphClient.reports()
    .getOneDriveActivityFileCounts("D7")
    .buildRequest()
    .get();

```