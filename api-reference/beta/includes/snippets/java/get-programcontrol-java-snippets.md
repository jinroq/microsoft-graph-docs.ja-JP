---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 832e278b20a2ee7f7afb0ff73337a4fde340af1e
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35875300"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IProgramControlCollectionPage programControls = graphClient.programControls()
    .buildRequest()
    .get();

```