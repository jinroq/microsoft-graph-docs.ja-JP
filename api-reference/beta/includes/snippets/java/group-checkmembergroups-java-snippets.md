---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6fac9e65d3861d094bcaeb8d462727f858c120f3
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35859022"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<String> groupIdsList = new LinkedList<String>();
groupIdsList.add("groupIds-value");

graphClient.groups("{id}")
    .checkMemberGroups(groupIdsList)
    .buildRequest()
    .post();

```