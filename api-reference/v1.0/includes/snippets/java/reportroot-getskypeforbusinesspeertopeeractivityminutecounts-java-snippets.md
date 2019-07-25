---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 580c285f174f6b5d3a62048adf0c6ef448eaf6b1
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35855674"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getSkypeForBusinessPeerToPeerActivityMinuteCounts('D7')
    .buildRequest()
    .get();

```