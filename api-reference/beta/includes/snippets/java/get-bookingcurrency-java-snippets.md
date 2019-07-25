---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 5bdc1912ff280a87dfa305b35660934baf8f495d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35865436"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

BookingCurrency bookingCurrency = graphClient.bookingCurrencies("USD")
    .buildRequest()
    .get();

```