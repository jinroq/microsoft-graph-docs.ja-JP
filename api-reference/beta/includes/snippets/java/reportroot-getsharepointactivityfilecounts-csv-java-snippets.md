---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 4dbae2dc0930b9ec30d8608528a825d12842232c
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35872890"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISiteActivitySummaryCollectionPage getSharePointActivityFileCounts = graphClient.reports()
    .getSharePointActivityFileCounts('D7')
    .buildRequest()
    .get();

```