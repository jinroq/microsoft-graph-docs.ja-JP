---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 0e92121a313b4a1a49c7cc01e053f16c9075d143
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35887193"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().messages("{id}")
    .buildRequest()
    .delete();

```