---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 198ff1602f6668ae42cb2588b99a3b48e73df31e
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35865520"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.bookingBusinesses("Contosolunchdelivery@M365B489948.onmicrosoft.com")
    .unpublish(bookingBusiness)
    .buildRequest()
    .post();

```