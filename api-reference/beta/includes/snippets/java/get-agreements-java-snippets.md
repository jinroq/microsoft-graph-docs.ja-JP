---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 8ee541c92e4538c156b0c6ab517520773d119132
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35855509"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IAgreementCollectionPage agreements = graphClient.agreements()
    .buildRequest()
    .get();

```