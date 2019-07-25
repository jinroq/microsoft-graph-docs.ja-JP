---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 7da9a76a3f94d9f335c5a6e873987b76904e715b
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35883894"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IContactCollectionPage contacts = graphClient.me().contactFolders("{id}").contacts()
    .buildRequest()
    .get();

```