---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: e8a82b4cb8d9eefd02d60b944433f5adf75f5fd2
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/30/2019
ms.locfileid: "35932840"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDriveItemCollectionPage bundles = graphClient.drive().bundles()
    .buildRequest()
    .get();

```