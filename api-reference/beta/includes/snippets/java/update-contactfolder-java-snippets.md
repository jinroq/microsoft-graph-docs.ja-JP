---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 30a9f2c9d8752894f0214521aa3d74b6618c2d01
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35863224"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ContactFolder contactFolder = new ContactFolder();
contactFolder.parentFolderId = "parentFolderId-value";
contactFolder.displayName = "displayName-value";

graphClient.me().contactFolders("{id}")
    .buildRequest()
    .patch(contactFolder);

```