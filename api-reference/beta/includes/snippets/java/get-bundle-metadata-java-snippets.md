---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 7083f5e9657a86cfeb7b04944a63c115fab4a4a9
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/30/2019
ms.locfileid: "35932853"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DriveItem driveItem = graphClient.drive().bundles("{bundle-id}")
    .buildRequest()
    .get();

```