---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 99422792015257db91b33557bd869a0cd639cbf5
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35857085"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String cancellationMessage = "Your appointment has been successfully cancelled. Please call us again.";

graphClient.bookingBusinesses("Contosolunchdelivery@M365B489948.onmicrosoft.com").appointments("AAMkADKoAAA=")
    .cancel(bookingAppointment,cancellationMessage)
    .buildRequest()
    .post();

```