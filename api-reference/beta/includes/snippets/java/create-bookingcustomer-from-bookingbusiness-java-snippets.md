---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 74a08c99b629b18c4b6dc1b7795d275003514d3b
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35865568"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

BookingCustomer bookingCustomer = new BookingCustomer();
bookingCustomer.displayName = "Joni Sherman";
bookingCustomer.emailAddress = "jonis@relecloud.com";

graphClient.bookingBusinesses("Contosolunchdelivery@M365B489948.onmicrosoft.com").customers()
    .buildRequest()
    .post(bookingCustomer);

```