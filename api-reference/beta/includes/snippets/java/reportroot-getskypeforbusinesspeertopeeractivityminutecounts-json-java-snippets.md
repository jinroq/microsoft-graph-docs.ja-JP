---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 518cacfd2fe31c887d5a1a7c3d7e5ee13add95a3
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35872047"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISkypeForBusinessPeerToPeerActivityMinuteCountsCollectionPage getSkypeForBusinessPeerToPeerActivityMinuteCounts = graphClient.reports()
    .getSkypeForBusinessPeerToPeerActivityMinuteCounts('D7')
    .buildRequest()
    .get();

```