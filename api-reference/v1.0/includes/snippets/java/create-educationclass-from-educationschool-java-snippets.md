---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: de9887678d93b1198cff78eeb7f853cb96ff6fe7
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35887674"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationClass educationClass = new EducationClass();
educationClass.additionalDataManager().put("@odata.id", new JsonPrimitive("https://graph.microsoft.com/v1.0/education/classes/11006"));

graphClient.education().schools("{school-id}").classes().references()
    .buildRequest()
    .post(educationClass);

```