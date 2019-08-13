---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 43e69bfdf40a8430586177373777f61e873b3a9a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36359773"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISharePointSiteUsagePagesCollectionPage getSharePointSiteUsagePages = graphClient.reports()
    .getSharePointSiteUsagePages("D7")
    .buildRequest()
    .get();

```