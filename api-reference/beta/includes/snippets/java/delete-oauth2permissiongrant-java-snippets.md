---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 8d0ec463e6bf4862b7cfa425a3b73e8735ab6498
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35878990"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.oAuth2Permissiongrants("{id}")
    .buildRequest()
    .delete();

```