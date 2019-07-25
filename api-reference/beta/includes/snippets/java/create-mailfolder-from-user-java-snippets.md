---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 913a7f648ab7dcb1d5cd376493dd421f783da703
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35866947"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MailFolder mailFolder = new MailFolder();
mailFolder.displayName = "displayName-value";

graphClient.me().mailFolders()
    .buildRequest()
    .post(mailFolder);

```