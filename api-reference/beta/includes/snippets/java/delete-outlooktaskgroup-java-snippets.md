---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 615933ad4daa113719f672263bb73d293989f7fd
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35877559"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().outlook().taskGroups("AAMkADIyAAAhrbe-AAA=")
    .buildRequest()
    .delete();

```