---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: b02ac8cdcfc8ab86b996035be6ceb5ec75ba1a06
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35880451"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.directory().deletedItems("{object-id}")
    .restore()
    .buildRequest()
    .post();

```