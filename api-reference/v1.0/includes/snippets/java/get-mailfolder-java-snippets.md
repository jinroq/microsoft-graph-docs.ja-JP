---
description: 自動生成されたファイル。 変更しないでください
ms.openlocfilehash: 00b5775d6efbc9fbbd2a26bbe651cfd365d31d1d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35856570"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MailFolder mailFolder = graphClient.me().mailFolders("AAMkAGVmMDEzM")
    .buildRequest()
    .get();

```