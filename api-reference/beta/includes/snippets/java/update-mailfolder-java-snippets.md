---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: cf1f6a4a152c4c00ba13baba56c451a6dc185b7a
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35880010"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MailFolder mailFolder = new MailFolder();
mailFolder.displayName = "displayName-value";

graphClient.me().mailFolders("AAMkAGVmMDEzM")
    .buildRequest()
    .patch(mailFolder);

```