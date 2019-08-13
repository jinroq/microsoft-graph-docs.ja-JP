---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: b5e925b9a3901745982bc12674860ab27aec7b05
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36358599"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IYammerActivityUserDetailCollectionPage getYammerActivityUserDetail = graphClient.reports()
    .getYammerActivityUserDetail("D7")
    .buildRequest()
    .get();

```