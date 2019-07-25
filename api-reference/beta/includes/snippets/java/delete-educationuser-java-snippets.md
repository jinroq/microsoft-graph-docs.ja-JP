---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 1474c5ca083e61de9a6de7d471060316699470de
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35859918"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().users("13019")
    .buildRequest()
    .delete();

```