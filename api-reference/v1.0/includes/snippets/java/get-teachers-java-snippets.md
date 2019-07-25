---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6526037c221ae232fb54dae01d065d9d5507ae1d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35881529"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IEducationUserCollectionPage teachers = graphClient.education().classes("{class-id}").teachers()
    .buildRequest()
    .get();

```