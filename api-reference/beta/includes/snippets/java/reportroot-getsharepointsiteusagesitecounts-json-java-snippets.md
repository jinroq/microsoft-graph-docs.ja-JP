---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 5bac74ee6a5dcf6206a05c6df183462fdeff4949
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36359752"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISharePointSiteUsageSiteCountsCollectionPage getSharePointSiteUsageSiteCounts = graphClient.reports()
    .getSharePointSiteUsageSiteCounts("D7")
    .buildRequest()
    .get();

```