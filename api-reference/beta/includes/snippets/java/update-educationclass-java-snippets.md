---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: e4946675fe3a25be6ddaf2797bbcc09738c78367
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35860512"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationClass educationClass = new EducationClass();
educationClass.description = "History - World History 1";
educationClass.displayName = "World History Level 1";

graphClient.education().classes("11014")
    .buildRequest()
    .patch(educationClass);

```