---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6290ccb2c9e107b52b555cefc8f65ab60251b85d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36358681"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IYammerActivitySummaryCollectionPage getYammerActivityCounts = graphClient.reports()
    .getYammerActivityCounts("D7")
    .buildRequest()
    .get();

```