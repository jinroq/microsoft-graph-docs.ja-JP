---
description: 自動生成されたファイル。 変更しないでください
ms.openlocfilehash: 3963a132f94ba67766b15eb473d0c8fb2b030afe
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35882747"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = graphClient.directoryObjects("{id}")
    .buildRequest()
    .get();

```