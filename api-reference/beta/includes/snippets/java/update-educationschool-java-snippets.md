---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 95fa3fc3dc072e0118bac9aa3a4cecfce20e8566
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35860194"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationSchool educationSchool = new EducationSchool();
educationSchool.displayName = "Fabrikam Arts High School";
educationSchool.description = "Magnate school for the arts. Los Angeles School District";

graphClient.education().schools("10002")
    .buildRequest()
    .patch(educationSchool);

```