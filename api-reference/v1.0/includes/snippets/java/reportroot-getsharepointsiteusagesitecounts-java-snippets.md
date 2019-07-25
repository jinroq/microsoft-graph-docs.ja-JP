---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6fd66d797fd4930ea64b8b517503c5e603675f71
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35893385"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getSharePointSiteUsageSiteCounts('D7')
    .buildRequest()
    .get();

```