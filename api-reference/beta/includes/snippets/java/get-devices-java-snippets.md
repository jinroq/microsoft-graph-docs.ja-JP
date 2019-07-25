---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6a654576e734efd5591cb3c316aa6f4426c96dca
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35862678"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDeviceCollectionPage devices = graphClient.devices()
    .buildRequest()
    .get();

```