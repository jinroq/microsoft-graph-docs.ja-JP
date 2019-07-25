---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 691b2b248297e999fa95a0bf60039241c2982a82
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35862096"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectorySetting directorySetting = graphClient.settings("{id}")
    .buildRequest()
    .get();

```