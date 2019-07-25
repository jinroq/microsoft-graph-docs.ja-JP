---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: ccd9cb97b3de1378c0aad284da4e72cc141e4b41
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35867556"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IAgreementAcceptanceCollectionPage agreementAcceptances = graphClient.me().agreementAcceptances()
    .buildRequest()
    .get();

```