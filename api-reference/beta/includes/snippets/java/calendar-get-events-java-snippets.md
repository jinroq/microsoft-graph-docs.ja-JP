---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 1d503ad2264a066b554c96e6b8c4166282417069
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35865078"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IEventCollectionPage events = graphClient.me().calendar().events()
    .buildRequest()
    .get();

```