---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 1922b44cfdb88754087a85573f722da8faf3be05
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35877369"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OutlookTaskFolder outlookTaskFolder = new OutlookTaskFolder();
outlookTaskFolder.name = "Volunteer";

graphClient.me().outlook().taskFolders()
    .buildRequest()
    .post(outlookTaskFolder);

```