---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: b4a566404ca99cec3b6f5c67de994741079c353a
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35862796"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Device device = graphClient.devices("{id}")
    .buildRequest()
    .get();

```