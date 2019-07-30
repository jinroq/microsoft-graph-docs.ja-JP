---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 7a7fd056bde8ba2de5f95148c2130000a18be694
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/30/2019
ms.locfileid: "35932833"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.drive().items("{bundle-id}")
    .buildRequest()
    .delete();

```