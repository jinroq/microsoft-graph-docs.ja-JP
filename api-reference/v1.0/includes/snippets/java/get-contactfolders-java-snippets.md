---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 4e920d176d34d3a2afda1eb279a8a1831bc03b69
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35886023"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IContactFolderCollectionPage contactFolders = graphClient.me().contactFolders()
    .buildRequest()
    .get();

```