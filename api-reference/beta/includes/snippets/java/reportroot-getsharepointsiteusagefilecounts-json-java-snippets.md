---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: e98a74fb8e3b4c7e24aef4d24be6522fc6f7441b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36359568"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISharePointSiteUsageFileCountsCollectionPage getSharePointSiteUsageFileCounts = graphClient.reports()
    .getSharePointSiteUsageFileCounts("D7")
    .buildRequest()
    .get();

```