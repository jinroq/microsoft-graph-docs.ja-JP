---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 63b2fa5aadcda770bbddcfb8cf7c9c1c9bbd8933
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35881087"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getOffice365ActivationCounts()
    .buildRequest()
    .get();

```