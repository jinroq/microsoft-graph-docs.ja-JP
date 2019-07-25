---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: f76dfe7e43fcbf143fa0817e7eab3034e21072b9
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35870891"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ITimeOffReasonCollectionPage timeOffReasons = graphClient.teams("{teamId}").schedule().timeOffReasons()
    .buildRequest()
    .get();

```