---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: cd2159512a5534b8084559c71f8d31b85ddb058f
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35872548"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISiteUsageStorageCollectionPage getSharePointSiteUsageStorage = graphClient.reports()
    .getSharePointSiteUsageStorage('D7')
    .buildRequest()
    .get();

```