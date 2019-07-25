---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 34eca7db2a510a5710de57129771b5758abab45a
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35873121"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISiteActivitySummaryCollectionPage getOneDriveActivityUserCounts = graphClient.reports()
    .getOneDriveActivityUserCounts('D7')
    .buildRequest()
    .get();

```