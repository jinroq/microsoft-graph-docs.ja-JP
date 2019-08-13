---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: cc0000d53c1389b91f10ac05f0457285dd0fbd09
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36359600"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISiteUsageStorageCollectionPage getSharePointSiteUsageStorage = graphClient.reports()
    .getSharePointSiteUsageStorage("D7")
    .buildRequest()
    .get();

```