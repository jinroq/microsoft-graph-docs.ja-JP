---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: e18d38dd7d7474e0093821903a63a1dcb53728c8
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35893357"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getSharePointSiteUsageStorage('D7')
    .buildRequest()
    .get();

```