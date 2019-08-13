---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: c5e79a12e703248063810ded08fa5088ad64a882
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36349365"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getSharePointSiteUsageStorage("D7")
    .buildRequest()
    .get();

```