---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: aef33d5a5e0ba3bcea324f968ba6c1f614e7a574
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35886766"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

GroupSetting groupSetting = graphClient.groupSettings("{id}")
    .buildRequest()
    .get();

```