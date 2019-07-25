---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 276ae39de8a474df3a8ccdb7e9dc6e7b87f37aa4
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35860582"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IEducationUserCollectionPage teachers = graphClient.education().classes("11023").teachers()
    .buildRequest()
    .get();

```