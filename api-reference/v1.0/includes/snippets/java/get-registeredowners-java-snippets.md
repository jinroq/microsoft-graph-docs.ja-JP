---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 0f8fde3b224d4d44fff89b28c4a5c260a9472a23
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35883441"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDirectoryObjectCollectionPage registeredOwners = graphClient.devices("{id}").registeredOwners()
    .buildRequest()
    .get();

```