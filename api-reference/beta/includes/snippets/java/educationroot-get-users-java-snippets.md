---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: b33918fa2cc13222ee3b37b3311704353559766d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35860454"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IEducationUserCollectionPage users = graphClient.education().users()
    .buildRequest()
    .get();

```