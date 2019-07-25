---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: e28f9b709c71cc8736798e4801a9ee6b36b7b3b5
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35862643"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Device device = new Device();
device.accountEnabled = false;

graphClient.devices("{id}")
    .buildRequest()
    .patch(device);

```