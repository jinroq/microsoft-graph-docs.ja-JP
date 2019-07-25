---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 9a438dab88ec5db4653dfcfa19080deddb012d7b
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35878756"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OnlineMeeting OnlineMeeting = graphClient.app().onlineMeetings("{id}")
    .buildRequest()
    .get();

```