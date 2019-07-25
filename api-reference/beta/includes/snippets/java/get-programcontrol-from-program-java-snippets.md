---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 86c3c5dff7df918c9247e98e7a951abf0649f055
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35875389"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IProgramControlCollectionPage controls = graphClient.programs("673a7379-9c38-4f01-bd9d-4fda7260b807").controls()
    .buildRequest()
    .get();

```