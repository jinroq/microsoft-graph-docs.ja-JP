---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: beb5bdd405bb55b0a6f8ec3a2309defd1cf77cf7
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/30/2019
ms.locfileid: "35931816"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.teams("{id}").installedApps("{id}")
    .buildRequest()
    .delete();

```