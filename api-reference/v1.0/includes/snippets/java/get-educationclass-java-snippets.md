---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: dedcc033e3b96e945a1bd80b8a55b7c8442f8455
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35886450"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationClass educationClass = graphClient.education().classes("{class-id}")
    .buildRequest()
    .get();

```