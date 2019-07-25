---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d6c5dd393054daf94b8777ff06368b97f070c481
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35855999"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IAccessReviewDecisionCollectionPage myDecisions = graphClient.accessReviews("2b83cc42-09db-46f6-8c6e-16fec466a82d").myDecisions()
    .buildRequest()
    .get();

```