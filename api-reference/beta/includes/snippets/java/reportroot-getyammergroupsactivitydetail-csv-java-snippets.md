---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 9b6d7edcc765f6e9878f8bd35996af5321a0386b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36358381"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IYammerGroupsActivityDetailCollectionPage getYammerGroupsActivityDetail = graphClient.reports()
    .getYammerGroupsActivityDetail("D7")
    .buildRequest()
    .get();

```