---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 3e63e2fec0bbc9fe8f8bd2ee29b7590b6e67f9d2
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35887746"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationSchool educationSchool = graphClient.education().schools("{school-id}")
    .buildRequest()
    .get();

```