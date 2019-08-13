---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 35fcd592162a68f6ba3b57bc59129f77b9edbad3
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36321780"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getSharePointSiteUsageFileCounts("D7")
    .buildRequest()
    .get();

```